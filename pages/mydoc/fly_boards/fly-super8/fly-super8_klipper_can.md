---
title: Fly-Super 8 Klipper CAN bus  firmware
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-Super 8 Klipper host"
sidebar: mydoc_sidebar
permalink: fly-super8_klipper_can.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-Super 8
firmware: can
ver: v1

micro: "STMicroelectronics STM32"
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"
com: "CAN bus on PB8/PB9"
appoffset: "32 KiB offset"
canspeed: "500000"




klipcom_img1: "fly-super8/fly-super8_klipper_menuconfig_can.png"
klipcom_cap1: "Klipper Menu Config CAN"

klipcom_img2: "fly-super8/fly-super8_klipper_canboot_burn.png"
klipcom_cap2: "Burn Klipper firmware over CAN bus"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"


---

## Configuring and installing Klipper for CAN bus

{% include custom/mcu/stm32/stm32_klipper_menuconfig.html %}

{% include custom/mcu/stm32/stm32_klipper_flash_canboot.html %}

{% include custom/can/sht_links.html %}

