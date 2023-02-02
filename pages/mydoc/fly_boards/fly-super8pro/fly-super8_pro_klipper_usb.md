---
title: Fly-Super 8 Pro MCU Klipper USB firmware
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-Super 8 Pro Klipper host"
sidebar: mydoc_sidebar
permalink: fly-super8_pro_klipper_usb.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-Super 8 Pro
firmware: usb
version: "V 1.2"
processor: "STM32H723"
offset: "128 KiB bootloader"
clock: "25 MHz crystal"

com: "USB on PA11/PA12"


klipcom_img1: "fly-super8_pro/fly-super8_pro_klipper_menuconfig_usb.png"
klipcom_cap1: "Klipper Menu Config USB"

klipcom_img2: "fly-super8/fly-super8_klipper_usb_burn.png"
klipcom_cap2: "Burn Klipper firmware over USB"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"


---

## Configuring and installing Klipper for USB

{% include custom/mcu/super8/super8_klipper_compile.html %}

{% include custom/can/sht_links.html %}