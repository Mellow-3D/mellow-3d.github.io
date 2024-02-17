---
title: Fly-E3v2 Klipper firmware for CAN
tags: []
keywords: 
last_updated: 17/02/2024
summary: "How to compile and install the klipper firmware running on a Fly-E3-v2 for CAN"
sidebar: mydoc_sidebar
permalink: fly_e3_v2_klipper_can.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-E3-v2
firmware: CANbus
mcu: "STM32"
kconfig_name: e3v2
low_level: "[*]"
architecture: "(STMicroelectronics STM32)"
processor: "(STM32F407)"
bootloader_offset: "(32KiB bootloader)"
clock: "(8 MHz crystal)"
communication: "(CAN bus (on PB8/PB9))"
can_bus_speed: "(1000000)"
gpio_startup: "()"
board_type: "mainboard"
klipper_file: "klipper.bin"
state: "install"

klipper_img1: "klipper/stm32f407_can_pb8pb9.png"
klipper_cap1: "Klipper Menu Config CAN"

klipper_img2: "fly-super8/flash-can_query.png"
klipper_cap2: "Flash Can Query"

klipper_img3: "fly-super8/fly-super8_klipper_canboot_burn.png"
klipper_cap3: "Burn Klipper firmware over CANbus"
---

## Configuring and installing Klipper for CAN bus

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_canboot_can.html %}

{% include custom/mcu/e3v2/fly_e3_v2_links.html %}
