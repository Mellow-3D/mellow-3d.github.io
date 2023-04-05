---
title: Fly-Super8Pro H723 CanBoot bootloader for CAN bus
tags: []
keywords: 
last_updated: 05/04/2023
summary: "Fly-Super8Pro H723 CanBoot bootloader for CAN bus"
sidebar: mydoc_sidebar
permalink: fly-super8_pro_h723_canboot_can.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: "Fly-Super8Pro H723"
firmware: can
ver: "V1.3" 
micro: "STMicroelectronics STM32"
processor: "STM32H723"
offset: "128 KiB bootloader"
clock: "25 MHz crystal"
com: "CAN bus on PB8/PB9"
appoffset: "128 KiB offset"
canspeed: "500000"
klipperurl: "[klipper firmware](./fly-super8_pro_h723_klipper_can.html)"
cancom_img1: "fly-super8_pro/fly-super8_pro_canboot_menuconfig_can.png"
cancom_cap1: "CanBoot Menu Config USB"
cancom_img2: "fly-super8/fly-super8_dfu_jumper.png"
cancom_cap2: "Fly-Super8Pro H723 DFU jumper"
canburn_img1: "fly-super8/fly-super8_pro_klipper_flash_fw_serial_usb.png"
canburn_cap1: "Fly-SuperPro8 H723 DFU lsusb"
canburn_img2: "fly-super8/fly-super8_canbus_usb_flash.png"
canburn_cap2: "Fly-Super8Pro H723 burn result"
---

## Configuring and installing CanBoot bootloader for CAN bus

{% include custom/mcu/stm32/stm32_canboot_menuconfig.html %}

{% include custom/mcu/stm32/stm32_canboot_flash_dfu.html  %}

{% include custom/can/sht_links.html %}