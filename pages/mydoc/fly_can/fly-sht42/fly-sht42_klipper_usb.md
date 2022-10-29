---
title: Configuring the Mellow SHT-42 canbus tool boards for Klipper on USB
tags: [content_types]
keywords: 
last_updated: 20/10/2022
summary: "Klipper Configuration for the Fly SHT-42 on USB"
sidebar: mydoc_sidebar
permalink: fly-sht42_klipper_usb.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: sht42
firmware: usb
version: v1

mcu: "SHT-42"

mcufile: "SHT-42"

klipcom_img1: "fly-sht36-42/sht_36_42_klipper_fw_usb_config.png"
klipcom_cap1: "Klipper Menu Config USB - update this image"

cancom_img1: "fly-sht36-42/sht_36_42_canbus_fw_usb_config.png"
cancom_cap1: "CanBoot Menu Config USB - update this image"

burn_img1:  "fly-sht36-42/sht_42_dfu_jumper.png"
burn_cap1:  "DFU jumper location" 

burn_img2:  "fly-sht36-42/sht_42_dfu_jumper_image.png"
burn_cap2:  "DFU jumper location"

burn_img3: "fly-sht36-42/sht-36_42_lsusb_screenshot.png"
burn_cap3: "lsusb Results"

burn_img4: "fly-sht36-42/sht-36_42_fw_burning_screenshot.png"
burn_cap4: "CanBoot burn complete - update this image"
---

{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}



## Setup steps

### Toolboard firmware

{% include custom/can/sht_canboot_compile.html %}

{% include custom/can/sht_canboot_burn.html %}

{% include custom/can/sht_klipper_compile.html %}

{% include custom/can/sht_klipper_configure.html %}

{% include custom/can/sht_links.html %}

