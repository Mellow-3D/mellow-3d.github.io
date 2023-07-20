---
title: Fly-407ZG MCU Klipper USB firmware
tags: []
keywords: 
last_updated: 19/07/2023
summary: "How to compile and install the klipper firmware running on a Fly-407ZG in USB mode"
sidebar: mydoc_sidebar
permalink: fly_407zg_klipper_usb.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-407ZG
firmware: usb
version: ""

micro: "STMicroelectronics STM32"
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"
com: "USB (on PA11/PA12)"
appoffset: "32 KiB offset"
canspeed: ""

klipcom_img1: "fly-super8/fly-super8_klipper_menuconfig_usb.png"
klipcom_cap1: "Klipper Menu Config USB"

klipcom_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipcom_cap2: "Burn Klipper firmware over USB"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"

kconfig_name: "407zg"
---

## Configuring and installing Klipper for USB

{% include tip.html content="To read more about the KCONFIG_CONFIG option, see [here](https://docs.vorondesign.com/community/howto/drachenkatze/automating_klipper_mcu_updates.html)" %}

{% include custom/mcu/stm32f4/klipper_menuconfig_usb.html %}

{% include custom/mcu/stm32f4/klipper_flash_canboot_usb.html %}

{% include custom/mcu/407zg/fly_407zg_links.html %}