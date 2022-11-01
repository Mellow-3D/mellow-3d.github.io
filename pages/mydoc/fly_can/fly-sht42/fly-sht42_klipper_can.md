---
title: Fly SHT42 Klipper configuration for CANBus
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Klipper configuration on the Fly SHT-42 V1 for CANBus"
sidebar: mydoc_sidebar
permalink: fly-sht42_klipper_can.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: sht42
firmware: can
version: v1

mcu: "SHT-42"

mcufile: "SHT-42"
com: "Canbus on PA8/PA9"

klipcom_img1: "fly-sht36-42/sht_36_42_klipper_fw_can_config.png"
klipcom_cap1: "Klipper Menu Config CAN - update this image"

cancom_img1: "fly-sht36-42/sht_36_42_canbus_fw_can_config.png"
cancom_cap1: "CanBoot Menu Config CAN - update this image"

burn_img1:  "fly-sht36-42/sht_42_dfu_jumper.png"
burn_cap1:  "DFU jumper location" 

burn_img2:  "fly-sht36-42/sht_42_dfu_jumper_image.png"
burn_cap2:  "DFU jumper location"

burn_img3: "fly-sht36-42/sht-36_42_lsusb_screenshot.png"
burn_cap3: "lsusb Results"

burn_img4: "fly-sht36-42/sht_36_42_canbus_usb_flash.png"
burn_cap4: "CanBoot burn complete"

---

{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}



## Setup steps

### Toolboard firmware

{% include custom/can/sht_canboot_compile.html %}

{% include custom/can/sht_canboot_burn.html %}

{% include custom/can/sht_klipper_compile.html %}

{% include custom/can/sht_klipper_configure.html %}

{% include custom/can/sht_links.html %}