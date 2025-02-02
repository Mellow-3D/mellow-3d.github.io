---
title: Updating Klipper Firmware on a Fly-D5 in USB to CAN Bridge mode
tags: []
keywords: 
last_updated: 19/02/2024
summary: "How to update the klipper firmware running on a Fly-D5 in USB to CAN Bridge mode"
sidebar: mydoc_sidebar
permalink: fly_d5_klipper_usb2can_updating.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-D5
firmware: USB2CAN
mcu: "STM32"
kconfig_name: d5
low_level: "[*]"
architecture: "(STMicroelectronics STM32)"
processor: "(STM32F072)"
bootloader_offset: "(8KiB bootloader)"
clock: "(8 MHz crystal)"
communication: "(USB to CAN bus bridge (USB on PA11/PA12))"
can_bus_interface: "(CAN bus (on PB8/PB9))"
usb_ids: ""
can_bus_speed: "(1000000)"
gpio_startup: "()"
board_type: "mainboard"
klipper_file: "klipper.bin"
state: "update"

klipper_img1: "klipper/stm32f072_usb2can_pb8pb9.png"
klipper_cap1: "Klipper Menu Config USB to CAN Bridge Mode"

klipper_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipper_cap2: "Burn Klipper firmware over USB"
---

## Configuring and installing Klipper for USB

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_katapult_usb.html %}

{% include custom/mcu/d5/fly_d5_links.html %}
