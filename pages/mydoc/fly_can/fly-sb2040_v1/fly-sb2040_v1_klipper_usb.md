---
title: Fly SB2040 V1 General Information
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Klipper Configuration the Fly SB2040 V1 on USB"
sidebar: mydoc_sidebar
permalink: fly-sb2040_v1_klipper_usb.html
folder: mydoc
comments: false
toc: false
datatable: true
---
## Overview 
Fly SB2040 V1



## Configuring the Mellow SHT-36 and SHT_42 tool boards for Klipper on USB. 



**This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device**

## Setup Steps

### Compile Toolboard Firmware
- ssh to your klipper host console
- cd to the klipper directory
```
cd klipper
```
- Run make clean
```
make clean
```
- Open menuconfig
```
make menuconfig
```
- Set the following options for CANBUS connection     
![Menu Config CANBUS](.\images\fly-sht36-42\sht_36_42_klipper_fw_usb_config.png)

- Quit and save the configuration

- Run the make command to compile the firmware

```
make
```
- You should now have a klipper.bin file at ~/klipper/out/

### Burn Firmware to Tool Board

- Install the boot jumper to the Boot0 pin and 3.3v pin as pictured. 

SHT-36 and SHT-42 DFU jumper location
![SHT-36 and SHT_42 burn jumper placement](.\images\fly-sht36-42\sht_36_42_dfu_jumper.png)

SHT-36 DFU Jumper
![SHT-36 burn jumper placement](.\images\fly-sht36-42\sht_36_dfu_jumper_image.png)

SHT-42 DFU Jumper
![SHT-42 burn jumper placement](.\images\fly-sht36-42\sht_42_dfu_jumper_image.png)

- Install the burning utility to your klipper host system
```
sudo apt install dfu-util -y
```
- Use a USB-C data cable to connect the SHT board to the klipper host, Make sure that the dfu jumper is installed before connecting the USB cable.      
- Run lsusb to see if the connection is successful, copy the USB ID in the blue box. Note that the board is in DFU mode. 
```
lsusb
```
![lsusb Results](.\images\fly-sht36-42\sht-36_42_lsusb_screenshot.png)

- Burn the firmware , replace 0483:df11 in the following command with the USB ID copied earlier
```
dfu-util -a 0 -d 0483:df11 --dfuse-address 0x08000000 -D ~/klipper/out/klipper.bin
```

- You should get a download progress bar and File downloaded successfuly when the burning is complete. 
![burn complete](.\images\fly-sht36-42\sht-36_42_fw_burning_screenshot.png)

- If the burn was sucessful remove the USB cable and the jumper from the Boot0 pin
- The tool board is now ready to install as a klipper MCU. 
**Repeat these steps if a klipper update requires flashing new firmware to the MCU. 


### Klipper Host configuration

- Klipper Host configuration
- Create a new file names can0 in the following folder /etc/network/interfaces.d
- Open a SSH session to your klipper host and run the following command. 

```
sudo  /etc/network/interfaces.d/can0
```
- Enter the following text and save the file

```
auto can0
iface can0 can static
    bitrate 500000
    up ifconfig $IFACE txqueuelen 1024
```
- You can set the bit rate to 250000, 500000 or 1000000. Be sure to use the same bitrate that you used when compiling the firmware. 



### Klipper CANBUS configuration
 - Finding the canbus_uuid for new micro-controllers¶
  Each micro-controller on the CAN bus is assigned a unique id based on the factory chip identifier encoded into each micro-controller. To find each micro-controller device id, make sure the hardware is powered and wired correctly, and then run the following the the host console. 


```
~/klippy-env/bin/python ~/klipper/scripts/canbus_query.py can0
```
  If uninitialized CAN devices are detected the above command will report lines like the following:


```
Found canbus_uuid=11aa22bb33cc
```
  Each device will have a unique identifier. In the above example, 11aa22bb33cc is the micro-controller's "canbus_uuid".

   Note that the canbus_query.py tool will only report uninitialized devices - if Klipper (or a similar tool) configures the device then it will no longer appear in the list.

 - Configuring Klipper
  Update the Klipper mcu configuration to use the CAN bus to communicate with the device - for example:

- Add the following lines to your printer.cfg file using your canbus_uuid
```
[mcu sht36]
canbus_uuid: 11aa22bb33cc
```
 - more needed here for configuring Can bus network settings. 

- USB Configuration
    - Run the following command at the Klipper host SSH console to get the serial path for the SHT board.
```
ls -l /dev/serial/by-id/
```
    - Note the ID containing 'stm32f072xb'

- Add the following lines to your printer.cfg file replacing the USB ID with the one you copied in the last section. 
```
[mcu sht36]
serial: /dev/serial/by-id/usb-Klipper_stm32f072xb_240024001757425835303220-if00
```

Impoprtant: THe SHT-36 has 120 ohm jumpers. If you board is the last device on the CAN bus it needs to have the jumpers installed.       
THe CANBUS needs to red 60 ohms across the L and H wires.       

![120ohmjumpers](.\images\fly-sht36-42\sht-36_120ohm_jumper.jpg)

