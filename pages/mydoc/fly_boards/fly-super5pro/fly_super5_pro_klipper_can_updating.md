---
title: Fly-Super5Pro Klipper firmware for CAN
tags: []
keywords: 
last_updated: 18/02/2024
summary: "How to compile and update the klipper firmware running on a Fly-Super5Pro for CAN"
sidebar: mydoc_sidebar
permalink: fly_super5_pro_klipper_can_updating.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-Super5Pro
firmware: CANbus
mcu: "STM32"
kconfig_name: super5pro
low_level: "[*]"
architecture: "(STMicroelectronics STM32)"
processor: "(STM32H723)"
bootloader_offset: "(128KiB bootloader (SKR SE BX v2.0))"
clock: "(25 MHz crystal)"
communication: "(CAN bus (on PB8/PB9))"
can_bus_speed: "(1000000)"
gpio_startup: "()"
board_type: "mainboard"
klipper_file: "klipper.bin"
state: "update"

klipper_img1: "klipper/stm32h723_can_pb8pb9.png"
klipper_cap1: "Klipper Menu Config CAN"

klipper_img2: "fly-super8/flash-can_query.png"
klipper_cap2: "Flash Can Query"

klipper_img3: "fly-super8/fly-super8_klipper_canboot_burn.png"
klipper_cap3: "Burn Klipper firmware over CANbus"
---

## Configuring and installing Klipper for CAN bus

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_katapult_can.html %}

{% include custom/mcu/super5_pro/fly_super5pro_links.html %}
