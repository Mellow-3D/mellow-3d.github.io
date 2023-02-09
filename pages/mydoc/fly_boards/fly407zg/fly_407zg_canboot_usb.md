---
title: Fly-407ZG CanBoot bootloader for USB
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-407ZG CanBoot bootloader for USB"
sidebar: mydoc_sidebar
permalink: fly-407zg_canboot_usb.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-407ZG
firmware: usb
ver: "" 

micro: "STMicroelectronics STM32"
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"
com: "USB on PA11/PA12"
appoffset: "32 KiB offset"
canspeed: ""

com: "USB on PA11/PA12"

klipperurl: "[Klipper for USB configuration section](fly-407zg_klipper_usb.html)"

klipperurl2: ""

cancom_img1: "fly-super8/fly-super8_canboot_menuconfig_usb.png"
cancom_cap1: "CanBoot Menuconfig"

canburn_img2: "fly-407zg/fly-f407zg_sdcard.png"
canburn_cap2: "Fly-407ZG SD card slot"

canburn_img1: "fly-407zg/fly-f407zg_reset.png"
canburn_cap1: "Fly-407ZG Reset button"

---

## Configuring and installing CanBoot bootloader for USB

{% include custom/mcu/stm32/stm32_canboot_menuconfig.html %}

{% include custom/mcu/stm32/stm32_canboot_flash_sd.html  %}

{% include custom/can/sht_links.html %}

