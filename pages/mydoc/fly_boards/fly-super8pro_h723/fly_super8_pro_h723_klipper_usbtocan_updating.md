---
title: Fly-Super8Pro H723 Klipper firmware in USB to Can Bridge Mode
tags: []
keywords: 
last_updated: 18/02/2024
summary: "How to compile and update the klipper firmware running on a Fly-Super8Pro H723 in USB to CAN Bridge Mode"
sidebar: mydoc_sidebar
permalink: fly_super8_pro_h723_klipper_usbtocan_updating.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-Super8Pro H723
firmware: USB2CAN
mcu: "STM32"
kconfig_name: super8proh723
low_level: "[*]"
architecture: "(STMicroelectronics STM32)"
processor: "(STM32H723)"
bootloader_offset: "(128KiB bootloader (SKR SE BX v2.0))"
clock: "(25 MHz crystal)"
communication: "(USB to CAN bus bridge (USB on PA11/PA12))"
can_bus_interface: "(CAN bus (on PB8/PB9))"
usb_ids: ""
can_bus_speed: "(1000000)"
gpio_startup: "()"
board_type: "mainboard"
klipper_file: "klipper.bin"
state: "update"

klipper_img1: "klipper/stm32h723_usb2can_pb8pb9.png"
klipper_cap1: "Klipper Menu Config USB to CAN Bridge Mode"

klipper_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipper_cap2: "Burn Klipper firmware over USB"
---

## Configuring and installing Klipper for USB to CAN Bridge Mode

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_katapult_usb.html %}

{% include custom/mcu/super8/fly_super8pro_links.html %}
