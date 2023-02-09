---
title: Fly 407ZG OEM bootloader
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly 407ZG restore OEM bootloader"
sidebar: mydoc_sidebar
permalink: fly-407zg_oem_bootloader.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly 407ZG
firmware: oem
ver: " " 

micro: "STMicroelectronics STM32"
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"
com: "USB on PA11/PA12"
appoffset: "32 KiB offset"
canspeed: ""

com: "USB on PA11/PA12"

klipperurl: "[Klipper configuration and flasing by SD card.](fly-407zg_klipper_sd.html)"

klipperurl2: "or [Klipper for USB to CAN bus configuration section](fly-super8_klipper_usbtocan.html)"

cancom_img1: "fly-407zg/fly_407zg_fix.png"
cancom_cap1: "Fly 407ZG DFU jumpers."

canburn_img1: "fly-407zg/stm32cube_connected.png"
canburn_cap1: "STM32Cube programmer connected"

canburn_img2: "fly-407zg/stm32cube_open_file.png"
canburn_cap2: "STM32Cube programmer file opened"

canburn_img3: "fly-407zg/stm32cube_burn.png"
canburn_cap3: "STM32Cube programmer burn firmware."

canburn_img4: "fly-407zg/stm32cube_open_file.png"
canburn_cap4: "STM32Cube programmer connected"

---

## installing the OEM bootloader.

### Download the OEM firmware
 - OEM firmware  file STM32.bin
can be downloaded [here.](hhttps://github.com/Mellow-3D/f407bootloader/releases)

{% include custom/mcu/stm32/stm32_oem_dfu_cube.html  %}

{% include custom/can/sht_links.html %}
