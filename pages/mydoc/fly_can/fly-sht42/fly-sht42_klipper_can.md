---
title: Fly SHT42 Klipper configuration for CAN bus
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Klipper configuration on the Fly SHT-42 V1 for CAN bus"
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
com: "CAN bus on PA8/PA9"

cancom_img1: "fly-sht36-42/sht_36_42_canbus_fw_can_config.png"
cancom_cap1: "CanBoot Menu Config CAN"

canburn_img1:  "fly-sht36-42/sht_42_dfu_jumper.png"
canburn_cap1:  "DFU jumper location" 

canburn_img2:  "fly-sht36-42/sht_42_dfu_jumper_image.png"
canburn_cap2:  "DFU jumper location"

canburn_img3: "fly-sht36-42/sht-36_42_lsusb_screenshot.png"
canburn_cap3: "lsusb Results"

canburn_img4: "fly-sht36-42/sht_36_42_canbus_usb_flash.png"
canburn_cap4: "CanBoot burn complete"

klipcom_img1: "fly-sht36-42/sht_36_42_klipper_fw_can_config.png"
klipcom_cap1: "Klipper Menu Config CAN"

klipcom_img4: "fly-sht36-42/sht_36_42_klipper_can_flash.png"
klipcom_cap4: "Klipper FW burn over can"

---

{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}



## Setup steps

### Toolboard firmware

{% include custom/can/sht_canboot_compile.html %}

{% include custom/can/sht_canboot_burn.html %}

{% include custom/can/sht_klipper_compile.html %}

{% include custom/can/sht_klipper_configure.html %}

{% include custom/can/sht_links.html %}

