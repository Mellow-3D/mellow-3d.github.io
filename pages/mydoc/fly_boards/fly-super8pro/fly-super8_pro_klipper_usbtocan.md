---
title: Fly-Super 8 Pro Klipper firmware in USB to Can Bridge
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-Super 8 Pro Klipper USB to CAN"
sidebar: mydoc_sidebar
permalink: fly-super8_pro_klipper_usbtocan.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-Super 8 Pro
firmware: usbtocan
version: v1

micro: "STMicroelectronics STM32"
processor: "STM32H723"
offset: "128 KiB bootloader"
clock: "25 MHz crystal"
com: "USB to CAN Bridge on PA11/PA12"
appoffset: "128 KiB offset"
canspeed: "500000"




klipcom_img1: "fly-super8_pro/fly-super8_pro_klipper_menuconfig_usb_can_bridge.png"
klipcom_cap1: "Klipper Menu Config USB to CAN"

klipcom_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipcom_cap2: "Burn Klipper firmware over USB"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"

---

## Configuring and installing Klipper for USB to CAN bridge mode

{% include warning.html content="Super 8 Version 1.0 does not support USB to CAN bridge mode." %}

{% include note.html content="If you are planning to use CANBoot bootloader with Klipper in USB to CAN bridge mode you will want to configure [CanBoot in USB mode](./fly-super8_pro_canboot_usb.html)" %}

{% include custom/mcu/stm32/stm32_klipper_menuconfig.html %}

{% include custom/mcu/stm32/stm32_klipper_flash_canboot.html %}

{% include custom/can/sht_links.html %}