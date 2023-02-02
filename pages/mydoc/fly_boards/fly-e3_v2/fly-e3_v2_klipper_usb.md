---
title: Fly-E3 v2 MCU Klipper USB firmware
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-E3 v2 Klipper host"
sidebar: mydoc_sidebar
permalink: fly-e3_v2_klipper_usb.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-E3 v2
firmware: usb
version: "V2"
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"

com: "USB on PA11/PA12"


klipcom_img1: "fly-super8/fly-super8_klipper_menuconfig_usb.png"
klipcom_cap1: "Klipper Menu Config USB"

klipcom_img2: "fly-super8/fly-super8_klipper_usb_burn.png"
klipcom_cap2: "Burn Klipper firmware over USB"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"


---

## Configuring and installing Klipper for USB

{% include custom/mcu/super8/super8_klipper_compile.html %}

{% include custom/can/sht_links.html %}