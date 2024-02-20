---
title: Fly-D5 MCU Klipper USB firmware
tags: []
keywords: 
last_updated: 19/02/2024
summary: "How to compile and update the klipper firmware running on a Fly-D5 in USB mode"
sidebar: mydoc_sidebar
permalink: fly_d5_klipper_usb_updating.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-D5
firmware: USB
mcu: "STM32"
kconfig_name: d5
low_level: "[*]"
architecture: "(STMicroelectronics STM32)"
processor: "(STM32F072)"
bootloader_offset: "(8KiB bootloader)"
clock: "(8 MHz crystal)"
communication: "(USB (on PA11/PA12))"
usb_ids: ""
gpio_startup: "()"
board_type: "mainboard"
klipper_file: "klipper.bin"
state: "update"

klipper_img1: "klipper/stm32f072_usb.png"
klipper_cap1: "Klipper Menu Config USB"

klipper_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipper_cap2: "Burn Klipper firmware over USB"
---

## Configuring and updating Klipper for USB

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_katapult_usb.html %}

{% include custom/mcu/d5/fly_d5_links.html %}
