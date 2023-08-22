---
title: Klipper Configuration for the Fly-ERCF-Easy-BRD-V1.1 on USB
tags: []
keywords: 
last_updated: 17/08/2023
summary: "Klipper Configuration for the Fly-ERCF-Easy-BRD-V1.1 on USB"
sidebar: mydoc_sidebar
permalink: fly_ercf_v1.1_klipper_usb_updating.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: Fly-ERCF-Easy-BRD-V1.1
firmware: USB
mcu: "rp2040"
version: v1
kconfig_name: ercfv1.1
low_level: "[*]"
architecture: "(Raspberry Pi RP2040)"
bootloader_offset: "(16KiB bootloader)"
communication: "(USB)"
usb_ids: ""
gpio_startup: "(gpio17)"
board_type: "toolboard"
klipper_file: "klipper.uf2"
120rurl: "./fly_ercf_v1.1_120r.html"
state: "update"

klipper_img1: "klipper/rp2040_usb_gpio17.png"
klipper_cap1: "Klipper Menu Config USB"

klipper_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipper_cap2: "Burn Klipper firmware over USB"

---
{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_canboot_usb.html %}

{% include custom/mcu/ercf_v1.1/ercf_v1.1_links.html %}
