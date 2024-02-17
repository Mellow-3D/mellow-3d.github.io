---
title: Klipper Configuration for the Fly-ADXL345-USB on USB
tags: []
keywords: 
last_updated: 21/08/2023
summary: "Klipper Configuration for the Fly-ADXL345-USB on USB"
sidebar: mydoc_sidebar
permalink: fly_adxl345_usb_klipper_usb.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: Fly-ADXL345-USB
firmware: USB
mcu: "rp2040"
version: v1
kconfig_name: adxl345
low_level: "[*]"
architecture: "(Raspberry Pi RP2040)"
bootloader_offset: "(16KiB bootloader)"
communication: "(USB)"
usb_ids: ""
gpio_startup: "()"
board_type: "toolboard"
klipper_file: "klipper.uf2"
state: "install"

klipper_img1: "klipper/rp2040_usb.png"
klipper_cap1: "Klipper Menu Config USB"

klipper_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipper_cap2: "Burn Klipper firmware over USB"

---
{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_katapult_usb.html %}

{% include custom/mcu/adxl345_usb/adxl345_usb_links.html %}
