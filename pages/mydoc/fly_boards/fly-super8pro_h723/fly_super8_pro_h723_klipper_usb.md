---
title: Fly-Super8Pro H723 MCU Klipper USB firmware
tags: []
keywords: 
last_updated: 18/02/2024
summary: "How to compile and install the klipper firmware running on a Fly-Super8Pro H723 in USB mode"
sidebar: mydoc_sidebar
permalink: fly_super8_pro_h723_klipper_usb.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-Super8Pro H723
firmware: USB
mcu: "STM32"
kconfig_name: super8proh723
low_level: "[*]"
architecture: "(STMicroelectronics STM32)"
processor: "(STM32H723)"
bootloader_offset: "(128KiB bootloader (SKR SE BX v2.0))"
clock: "(25 MHz crystal)"
communication: "(USB (on PA11/PA12))"
usb_ids: ""
gpio_startup: "()"
board_type: "mainboard"
klipper_file: "klipper.bin"
state: "install"

klipper_img1: "klipper/stm32h723_usb.png"
klipper_cap1: "Klipper Menu Config USB"

klipper_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipper_cap2: "Burn Klipper firmware over USB"
---

## Configuring and installing Klipper for USB

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_katapult_usb.html %}

{% include custom/mcu/super8/fly_super8pro_links.html %}
