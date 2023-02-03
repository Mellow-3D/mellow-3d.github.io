---
title: Fly Super 8 CanBoot bootloader for CAN bus
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly Super 8 CanBoot bootloader for CAN bus"
sidebar: mydoc_sidebar
permalink: fly-super8_canboot_can.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-Super 8
firmware: can
ver: "V 1.2" 

micro: "STMicroelectronics STM32"
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"
com: "CAN bus on PB8/PB9"
appoffset: "32 KiB offset"
canspeed: "500000"

klipperurl: "[Klipper for CAN bus configuration section](fly-super8_klipper_can.html)"



cancom_img1: "fly-super8/fly-super8_canboot_menuconfig_can.png"
cancom_cap1: "CanBoot Menuconfig"

cancom_img2: "fly-super8/fly-super8_sd.png"
cancom_cap2: "Fly Super 8 SD card slot"

canburn_img2: "fly-super8/fly-super8_sd.png"
canburn_cap2: "Fly Super 8 SD card slot"

canburn_img1: "fly-super8/fly-super8_reset.png"
canburn_cap1: "Fly Super 8 Reset button"

---

## Configuring and installing CanBoot bootloader for CAN bus

{% include custom/mcu/stm32/stm32_canboot_menuconfig.html %}

{% include custom/mcu/stm32/stm32_canboot_flash_sd.html  %}

{% include custom/can/sht_links.html %}

