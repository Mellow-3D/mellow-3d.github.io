---
title: Klipper Configuration for the Fly SB2040 V1 on USB
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Klipper Configuration for the Fly SB2040 V1 on USB"
sidebar: mydoc_sidebar
permalink: fly-sb2040_klipper_usb.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: Fly-S2040
firmware: usb
version: v1

mcu: "Fly-SB2040"

mcufile: "SB2040"
com: "USB"

cancom_img1: "fly-sb2040_v1/sb2040_canboot_menuconfig_usb.png"
cancom_cap1: "CanBoot Menu Config USB"

canburn_img1:  "fly-sb2040_v1/sb2040_button.png"
canburn_cap1:  "SB2040 boot button location" 

canburn_img2:  "fly-sb2040_v1/sb2040_boot_button_image.png"
canburn_cap2:  "SB2040 boot button location"

canburn_img3: "fly-sb2040_v1/fly-sb2040_lsusb_screenshot.png"
canburn_cap3: "lsusb Results"

canburn_img4: "fly-sb2040_v1/sb2040_canboot_uf2_burn.png"
canburn_cap4: "CanBoot firmware burn is complete when /mnt unmounts"

klipcom_img1: "fly-sb2040_v1/sb2040_klipper_menuconfig_usb.png"
klipcom_cap1: "Klipper Menu Config on USB"

klipcom_img4: "fly-sb2040_v1/sb2040_klipper_canboot_usb_burn.png"
klipcom_cap4: "Klipper FW burn over USB"
---
{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}



## Setup steps

### Toolboard firmware

{% include custom/can/sb2040_canboot_compile.html %}

{% include custom/can/sb2040_canboot_burn.html %}

{% include custom/can/sb2040_klipper_compile.html %}

{% include custom/can/sb2040_klipper_configure.html %}

{% include custom/can/sht_links.html %}
