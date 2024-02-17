---
title: Installing Klipper Firmware on a Fly-CDYv2 in USB mode
tags: []
keywords: 
last_updated: 17/02/2024
summary: "How to compile and install the klipper firmware running on a Fly-CDYv2 in USB mode"
sidebar: mydoc_sidebar
permalink: fly_cdyv2_klipper_usb.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-CDYv2
firmware: USB
mcu: "STM32"
kconfig_name: cdyv2
low_level: "[*]"
architecture: "(STMicroelectronics STM32)"
processor: "(STM32F407)"
bootloader_offset: "(32KiB bootloader)"
clock: "(8 MHz crystal)"
communication: "(USB (on PA11/PA12))"
usb_ids: ""
gpio_startup: "()"
board_type: "mainboard"
klipper_file: "klipper.bin"
state: "install"

klipper_img1: "klipper/stm32f407_usb.png"
klipper_cap1: "Klipper Menu Config USB"

klipburn_img1: "fly-cdy_v3/fly-cdy_v3_sd_card.png"
klipburn_cap1: "FLy-CDYv2 SD card"

klipburn_img2: "fly-cdy_v3/fly-cdy_v3_reset.png"
klipburn_cap2: "Fly-CDYv2 reset"
---

## Configuring and installing Klipper for USB

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_sd_card.html %}

{% include custom/mcu/cdyv2/fly_cdyv2_links.html %}
