---
title: Fly-Super8Pro H723 MCU Klipper USB firmware
tags: []
keywords: 
last_updated: 05/04/2023
summary: "Fly-Super8Pro H723 Klipper host"
sidebar: mydoc_sidebar
permalink: fly-super8_pro_h723_klipper_usb.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: "Fly-Super8Pro H723"
firmware: usb
version: "V1.3"
notetag: "prousb"
micro: "STMicroelectronics STM32"
processor: "STM32H723"
offset: "128 KiB bootloader"
clock: "25 MHz crystal"
com: "USB on PA11/PA12"
appoffset: "128 KiB offset"
canspeed: ""
klipcom_img1: "fly-super8_pro/fly-super8_pro_klipper_menuconfig_usb.png"
klipcom_cap1: "Klipper Menu Config USB"
klipcom_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipcom_cap2: "Burn Klipper firmware over USB"
klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"
---

## Configuring and installing Klipper for USB

{% include custom/mcu/stm32/stm32_klipper_menuconfig.html %}

{% include custom/mcu/stm32/stm32_klipper_flash_canboot.html %}

{% include custom/can/sht_links.html %}