---
title: Fly SHT 36 V2 Klipper configuration for CAN bus
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Klipper configuration on the Fly SHT-36 V2 for CAN bus"
sidebar: mydoc_sidebar
permalink: fly-sht36_v2_klipper_can.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: sht36v2
firmware: can
version: v1

mcu: "SHT-36 V2"

mcufile: "SHT-36V2"
com: "CAN bus on PB8/PB9"

cancom_img1: "fly-sht36_v2/sht36_v2_canboot_config_stmf072.png"
cancom_cap1: "STM32F072 CanBoot Menu Config CAN"

cancom_img2: "fly-sht36_v2/sht36_v2_canboot_config_stmf103.png"
cancom_cap2: "STM32F103 CanBoot Menu Config CAN"

canburn_img1:  "fly-sht36_v2/sht36_v2_boot0.png"
canburn_cap1:  "DFU jumper location" 

canburn_img3: "fly-sht36-42/sht-36_42_lsusb_screenshot.png"
canburn_cap3: "lsusb Results"

canburn_img4: "fly-sht36-42/sht_36_42_canbus_usb_flash.png"
canburn_cap4: "CanBoot burn complete"

klipcom_img1: "fly-sht36_v2/sht36_v2_klipper_config_stmf072.png"
klipcom_cap1: "STM32F072 Klipper Menu Config CAN"

klipcom_img2: "fly-sht36_v2/sht36_v2_klipper_config_stmf103.png"
klipcom_cap2: "STM32F103 Klipper Menu Config CAN"

klipcom_img4: "fly-sht36-42/sht_36_42_klipper_can_flash.png"
klipcom_cap4: "Klipper FW burn over CAN"

---

{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}



## Setup steps

### Toolboard firmware

{% include custom/can/sht_v2_canboot_compile.html %}

{% include custom/can/sht_v2_canboot_burn.html %}

{% include custom/can/sht_v2_klipper_compile.html %}

{% include custom/can/sht_v2_klipper_configure.html %}

{% include custom/can/sht_links.html %}

