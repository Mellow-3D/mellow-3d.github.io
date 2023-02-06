---
title: Fly-CDY V3 MCU Klipper USB firmware
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-CDY V3 Klipper host"
sidebar: mydoc_sidebar
permalink: fly-cdy_v3_klipper_usb.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-CDY V3
firmware: usb
version: "V3"

micro: "STMicroelectronics STM32"
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"
com: "USB on PA11/PA12"
appoffset: "32 KiB offset"
canspeed: ""


klipcom_img1: "fly-super8/fly-super8_klipper_menuconfig_usb.png"
klipcom_cap1: "Klipper Menu Config USB"

klipcom_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipcom_cap2: "Burn Klipper firmware over USB"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"

klipburn_img1: "fly-cdy_v3/fly-cdy_v3_sd_card.png"
klipburn_cap1: "FLy-CDY V3 SD card"

klipburn_img2: "fly-cdy_v3/fly-cdy_v3_reset.png"
klipburn_cap2: "Fly-CDY V3 reset"

---

## Configuring and installing Klipper for USB

{% include custom/mcu/stm32/stm32_klipper_menuconfig.html %}

{% include custom/mcu/stm32/stm32_klipper_flash_sd.html %}

{% include custom/can/sht_links.html %}