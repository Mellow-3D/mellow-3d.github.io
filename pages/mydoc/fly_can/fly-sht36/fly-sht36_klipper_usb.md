---
title: Configuring the Mellow SHT-36 canbus tool boards for Klipper on USB
tags: [content_types]
keywords: 
last_updated: 20/10/2022
summary: "Klipper Configuration for the Fly SHT-36 V1 on USB"
sidebar: mydoc_sidebar
permalink: fly-sht36_klipper_usb.html
folder: mydoc
comments: false
toc: false
datatable: true
---

{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}


* TOC
{:toc}

## Setup steps

### Toolboard firmware

#### Compile CanBoot firmware   

- ssh to your klipper host console

- Install the burning utility to your klipper host system
```
sudo apt install dfu-util -y
```

- Clone the CanBoot firmware to your Klipper Host
```
cd ~/
git clone https://github.com/Arksine/CanBoot
```

- cd to the Canboot directory
```
cd Canboot
```
- Run make clean
```
make clean
```
- Open menuconfig
```
make menuconfig
```
- Set the following options for USB connection     
    {% 
    include image.html 
    file="fly-sht36-42\sht_36_42_klipper_fw_usb_config.png"
    url=".\images\fly-sht36-42\sht_36_42_klipper_fw_usb_config.png" 
    alt="Menu Config USB"
    caption="CanBoot Menu Config USB - update this image" 
    %}

- Quit and save the configuration

- Run the make command to compile the firmware
```
make
```
- You should now have a canboot.bin file at ~/CanBoot/out/

#### Burn CanBoot firmware to tool board

- Install the boot jumper to the Boot0 pin and 3.3v pin as pictured. 

    {% 
    include image.html 
    file="fly-sht36-42\sht_36_42_dfu_jumper.png"
    url=".\images\fly-sht36-42\sht_36_42_dfu_jumper.png" 
    alt="SHT-36 and SHT_42 burn jumper placement"
    caption="SHT-36 and SHT-42 DFU jumper location" 
    %}
 

    {% 
    include image.html 
    file="fly-sht36-42\sht_36_dfu_jumper_image.png" 
    url=".\images\fly-sht36-42\sht_36_dfu_jumper_image.png"
    alt="SHT-36 burn jumper placement"
    caption="SHT-36 DFU Jumper" 
    %}

    {% 
    include image.html 
    file="fly-sht36-42\sht_42_dfu_jumper_image.png" 
    url=".\images\fly-sht36-42\sht_42_dfu_jumper_image.png"
    alt="SHT-42 burn jumper placement"
    caption="SHT-42 DFU Jumper" 
    %}


- Use a USB-C data cable to connect the SHT board to the klipper host, Make sure that the dfu jumper is installed before connecting the USB cable.      
- Run lsusb to see if the connection is successful, copy the USB ID in the blue box. Note that the board is in DFU mode. 
```
lsusb
```
    {% 
    include image.html 
    file="fly-sht36-42\sht-36_42_lsusb_screenshot.png" 
    url=".\images\fly-sht36-42\sht-36_42_lsusb_screenshot.png"
    alt="lsusb Results"
    caption="lsusb Results" 
    %}

- Erase and Burn the firmware , replace 0483:df11 in the following command with the USB ID copied earlier
```
sudo dfu-util -a 0 -D ~/CanBoot/out/canboot.bin --dfuse-address 0x08000000:force:mass-erase:leave -d 0483:df11
```

- You should get a download progress bar and File downloaded successfuly when the burning is complete. 
    {% 
    include image.html 
    file="fly-sht36-42\sht-36_42_fw_burning_screenshot.png" 
    url=".\images\fly-sht36-42\sht-36_42_fw_burning_screenshot.png"
    alt="burn complete"
    caption="CanBoot burn complete - update this image" 
    %}

- If the burn was sucessful remove the jumper from the Boot0 pin and power cycle the printer or jsut the SHT-36 by upluging the USB and 24v power then pluging them back in again. 
- The tool board is now ready to install as a klipper MCU. 
 

#### Compile Klipper firmware and flash with CanBoot  
{% include note.html content="Repeat these steps if a klipper update requires flashing new firmware to the MCU." %}

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
- Set the following options for USB connection     
    {% 
    include image.html 
    file="fly-sht36-42\sht_36_42_klipper_fw_usb_config.png"
    url=".\images\fly-sht36-42\sht_36_42_klipper_fw_usb_config.png" 
    alt="Menu Config USB"
    caption="Menu Config USB" 
    %}

- Quit and save the configuration

- Find the Serial ID
```
ls -l /dev/serial/by-id/
```
- Copy the ID containing 'stm32f072xb'

- Run the make flash command to compile the firmware
```
make flash FLASH_DEVICE={paste your serial by id here}
```
- You should now have a klipper.bin file at ~/klipper/out/


### USB configuration
- Run the following command at the Klipper host SSH console to get the serial path for the SHT board.

```
ls -l /dev/serial/by-id/
```
- Note the ID containing 'stm32f072xb'

*add screen shot here*

- Add the following lines to your printer.cfg file replacing the USB ID with the one you copied in the last section. 
```
[mcu sht36]
serial: /dev/serial/by-id/{copy usb serial ID here}
```

