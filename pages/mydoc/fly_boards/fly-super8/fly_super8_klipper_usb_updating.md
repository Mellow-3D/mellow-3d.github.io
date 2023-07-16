---
title: Updating Klipper Firmware on a Fly-Super8 in USB mode
tags: []
keywords: 
last_updated: 16/07/2023
summary: "How to update the klipper firmware running on a Fly-Super8 in USB mode"
sidebar: mydoc_sidebar
permalink: fly_super8_klipper_usb.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-Super 8
firmware: usb
version: "V 1.2"

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

kconfig_name: "super8"
---

## Configuring and installing Klipper for USB

{% include tip.html content="To read more about the KCONFIG_CONFIG option, see [here](https://docs.vorondesign.com/community/howto/drachenkatze/automating_klipper_mcu_updates.html)" %}

{% include custom/mcu/stm32f4/klipper_menuconfig_usb_updating.html %}

{% include custom/mcu/stm32f4/klipper_flash_canboot_usb_updating.html %}

{% include custom/mcu/super8/fly_super8_links.html %}