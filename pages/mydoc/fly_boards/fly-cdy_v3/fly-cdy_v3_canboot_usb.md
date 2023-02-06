---
title: Fly CDY V3 CanBoot bootloader for USB
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly CDY v3 CanBoot bootloader for USB"
sidebar: mydoc_sidebar
permalink: fly-cdy_v3_canboot_usb.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly CDY v3
firmware: usb
ver: "V3" 

micro: "STMicroelectronics STM32"
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"
com: "USB on PA11/PA12"
appoffset: "32 KiB offset"
canspeed: ""

com: "USB on PA11/PA12"

klipperurl: "[Klipper for USB configuration section](fly-cdy_v3_klipper_usb.html)"

klipperurl2: ""

com: "USB on PA11/PA12"

cancom_img1: "fly-super8/fly-super8_canboot_menuconfig_usb.png"
cancom_cap1: "CanBoot Menu Config USB"

canburn_img2: "fly-cdy_v3/fly-cdy_v3_sd_card.png"
canburn_cap2: "Fly CDCY V3 SD card"

canburn_img1: "fly-cdy_v3/fly-cdy_v3_reset.png"
canburn_cap1: "Fly CDCY V3 reset button"

---

## Configuring and installing CanBoot bootloader for USB


{% include custom/mcu/stm32/stm32_canboot_compile.html %}

{% include custom/mcu/stm32/stm32_canboot_flash_sd.html %}

{% include custom/can/sht_links.html %}

