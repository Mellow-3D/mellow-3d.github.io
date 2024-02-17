---
title: Fly-E3-v2 MCU Klipper USB firmware
tags: []
keywords: 
last_updated: 15/07/2023
summary: "How to compile and update the klipper firmware running on a Fly-E3-v2 in USB mode"
sidebar: mydoc_sidebar
permalink: fly_e3_v2_klipper_usb_updating.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-E3-v2
firmware: USB
mcu: "STM32"
kconfig_name: e3v2
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
state: "update"

klipper_img1: "klipper/stm32f407_usb.png"
klipper_cap1: "Klipper Menu Config USB"

klipper_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipper_cap2: "Burn Klipper firmware over USB"
---

## Configuring and updating Klipper for USB

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_katapult_usb.html %}

{% include custom/mcu/e3v2/fly_e3_v2_links.html %}
