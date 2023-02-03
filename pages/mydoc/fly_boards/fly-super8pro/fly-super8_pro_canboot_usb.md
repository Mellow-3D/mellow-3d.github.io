---
title: Fly Super 8 Pro CanBoot bootloader for USB
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly Super 8 Pro CanBoot Probootloader for USB"
sidebar: mydoc_sidebar
permalink: fly-super8_pro_canboot_usb.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly Super 8 Pro
firmware: usb
ver: "V 1.2" 

micro: "STMicroelectronics STM32"
processor: "STM32H723"
offset: "128 KiB bootloader"
clock: "25 MHz crystal"
com: "USB on PA11/PA12"
appoffset: "128 KiB offset"
canspeed: ""


klipperurl: "[klipper firmware](./fly-super8_pro_canboot_usb.html)"



cancom_img1: "fly-super8_pro/fly-super8_pro_canboot_menuconfig_usb.png"
cancom_cap1: "CanBoot Menu Config USB"

cancom_img2: "fly-super8/fly-super8_dfu_jumper.png"
cancom_cap2: "Fly Super 8 Pro DFU jumper"

canburn_img1: "fly-super8/fly-super8_pro_klipper_flash_fw_serial_usb.png"
canburn_cap1: "Fly Super 8 Pro dfu lsusb"

canburn_img2: "fly-super8/fly-super8_canbus_usb_flash.png"
canburn_cap2: "Fly Super 8 Pro burn result"

---

## Configuring and installing CanBoot bootloader for USB

{% include custom/mcu/stm32/stm32_canboot_menuconfig.html %}

{% include custom/mcu/stm32/stm32_canboot_flash_dfu.html  %}

{% include custom/can/sht_links.html %}

