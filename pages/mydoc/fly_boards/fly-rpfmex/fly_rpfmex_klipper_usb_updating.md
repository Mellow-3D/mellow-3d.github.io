---
title: Fly-RPFMex MCU Klipper USB firmware
tags: []
keywords: 
last_updated: 17/02/2024
summary: "How to compile and update the klipper firmware running on a Fly-RPFMex in USB mode"
sidebar: mydoc_sidebar
permalink: fly_rpfmex_klipper_usb_updating.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-RPFMex
firmware: USB
mcu: "rp2040"
version: v1
kconfig_name: rpfmex
low_level: "[*]"
architecture: "(Raspberry Pi RP2040)"
bootloader_offset: "(16KiB bootloader)"
communication: "(USB)"
usb_ids: ""
gpio_startup: "(gpio24)"
board_type: "toolboard"
klipper_file: "klipper.uf2"
state: "update"

klipper_img1: "klipper/rp2040_usb_gpio24.png"
klipper_cap1: "Klipper Menu Config USB"

klipper_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipper_cap2: "Burn Klipper firmware over USB"

---
{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_katapult_usb.html %}

{% include custom/mcu/rpfmex/fly_rpfmex_links.html %}
