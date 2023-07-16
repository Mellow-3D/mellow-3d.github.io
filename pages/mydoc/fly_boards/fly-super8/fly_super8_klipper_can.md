---
title: Fly-Super8 Klipper CANbus firmware
tags: []
keywords: 
last_updated: 16/07/2023
summary: "Fly-Super8 Klipper host"
sidebar: mydoc_sidebar
permalink: fly_super8_klipper_can.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-Super8
firmware: can
ver: v1

processor: "STM32F407"
com: "CAN bus (on PB8/PB9)"
micro: "STMicroelectronics STM32"
offset: "32KiB bootloader"
clock: "8 MHz crystal"
appoffset: "32KiB offset"
canspeed: "500000"

klipcom_img1: "fly-super8/fly-super8_klipper_menuconfig_can.png"
klipcom_cap1: "Klipper Menu Config CAN"

klipcom_img2: "fly-super8/fly-super8_klipper_canboot_burn.png"
klipcom_cap2: "Burn Klipper firmware over CAN bus"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"

kconfig_name: "super8"
---

## Configuring and installing Klipper for CANbus

{% include tip.html content="To read more about the KCONFIG_CONFIG option, see [here](https://docs.vorondesign.com/community/howto/drachenkatze/automating_klipper_mcu_updates.html)" %}

{% include custom/mcu/stm32f4/klipper_menuconfig_can.html %}

{% include custom/mcu/stm32f4/klipper_flash_canboot_can.html %}

{% include custom/mcu/super8/fly_super8_links.html %}

