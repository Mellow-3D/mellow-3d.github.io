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
boardname: sht36
firmware: usb
---

{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}


* TOC
{:toc}

## Setup steps

### Toolboard firmware

{% include custom/can/sht_canboot_compile.html %}

{% include custom/can/sht_canboot_burn.html %}


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

