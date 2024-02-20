---
title: Updating Klipper Firmware on a Fly-D5 in CANbus mode
tags: []
keywords: 
last_updated: 19/02/2024
summary: "How to update the klipper firmware running on a Fly-D5 in CANbus mode"
sidebar: mydoc_sidebar
permalink: fly_d5_klipper_can_updating.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-D5
firmware: CANbus
mcu: "STM32"
kconfig_name: d5
low_level: "[*]"
architecture: "(STMicroelectronics STM32)"
processor: "(STM32072)"
bootloader_offset: "(8KiB bootloader)"
clock: "(8 MHz crystal)"
communication: "(CAN bus (on PB8/PB9))"
can_bus_speed: "(1000000)"
gpio_startup: "()"
board_type: "mainboard"
klipper_file: "klipper.bin"
state: "update"

klipper_img1: "klipper/stm32f072_can_pb8pb9.png"
klipper_cap1: "Klipper Menu Config CAN"

klipper_img2: "fly-super8/flash-can_query.png"
klipper_cap2: "Flash Can Query"

klipper_img3: "fly-super8/fly-super8_klipper_canboot_burn.png"
klipper_cap3: "Burn Klipper firmware over CANbus"
---

## Configuring and installing Klipper for CAN bus

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_katapult_can.html %}

{% include custom/mcu/d5/fly_d5_links.html %}
