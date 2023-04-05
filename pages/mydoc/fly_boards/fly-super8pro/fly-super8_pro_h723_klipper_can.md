---
title: Fly-Super8Pro H723 Klipper CANbus firmware
tags: []
keywords: 
last_updated: 05/04/2023
summary: "Fly-Super8Pro H723 Klipper host"
sidebar: mydoc_sidebar
permalink: fly-super8_pro_h723_klipper_can.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: "Fly-Super8Pro H723"
firmware: can
ver: V1.3
micro: "STMicroelectronics STM32"
processor: "STM32H723"
offset: "128 KiB bootloader"
clock: "25 MHz crystal"
com: "CAN on PB8/PB9"
canspeed: "500000"
klipcom_img1: "fly-super8_pro/fly-super8_pro_klipper_menuconfig_can.png"
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

