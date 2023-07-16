---
title: Fly-E3-v2 Klipper CANbus firmware
tags: []
keywords: 
last_updated: 15/07/2023
summary: "Fly-E3-v2 Klipper host"
sidebar: mydoc_sidebar
permalink: fly_e3_v2_klipper_can.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-E3-v2
firmware: can
ver: v2
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"
micro: "STMicroelectronics STM32"
com: "CAN on PB8/PB9"
canspeed: "500000"

klipcom_img1: "fly-super8/fly-super8_klipper_menuconfig_can.png"
klipcom_cap1: "Klipper Menu Config CANbus"

klipcom_img2: "fly-super8/fly-super8_klipper_canboot_burn.png"
klipcom_cap2: "Burn Klipper firmware over CANbus"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"

kconfig_name: "e3v2"
---

## Configuring and installing Klipper for CANbus

{% include tip.html content="To read more about the KCONFIG_CONFIG option, see [here](https://docs.vorondesign.com/community/howto/drachenkatze/automating_klipper_mcu_updates.html)" %}

{% include custom/mcu/stm32f4/klipper_menuconfig_can.html %}

{% include custom/mcu/stm32f4/klipper_flash_canboot_can.html %}

{% include custom/mcu/e3v2/fly_e3_v2_links.html %}
