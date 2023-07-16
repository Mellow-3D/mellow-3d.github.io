---
title: Fly-Super8 CanBoot bootloader for USB
tags: []
keywords: 
last_updated: 16/07/2023
summary: "Fly-Super8 CanBoot bootloader for USB"
sidebar: mydoc_sidebar
permalink: fly_super8_canboot_usb.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-Super8
firmware: usb
ver: "V 1.2" 

processor: "STM32F407"
com: "USB (on PA11/PA12)"
micro: "STMicroelectronics STM32"
offset: "32KiB bootloader"
clock: "8 MHz crystal"
appoffset: "32KiB offset"

com: "USB on PA11/PA12"

klipperurl: "[Klipper for USB configuration section](fly_super8_klipper_usb.html)"

klipperurl2: "or [Klipper for USB to CAN bus configuration section](fly_super8_klipper_usbtocan.html)"

cancom_img1: "fly-super8/fly-super8_canboot_menuconfig_usb.png"
cancom_cap1: "CanBoot Menuconfig"

cancom_img2: "fly-super8/fly-super8_sd.png"
cancom_cap2: "Fly-Super8 SD card slot"

cancom_img3: "fly-super8/fly-super8_reset.png"
cancom_cap3: "Fly-Super8 Reset button"

canburn_img1: "fly-super8/fly-super8_pro_klipper_flash_fw_serial_usb.png"
canburn_cap1: "Fly-Super8 dfu lsusb"

canburn_img2: "fly-super8/fly-super8_canbus_usb_flash.png"
canburn_cap2: "Fly-Super8 burn result"

installKlipperURL: "./fly_super8_klipper_usb2can.html"
installKlipperName: "Klipper for USB to CAN Bridge Mode configuration section"
---

## Configuring and installing CanBoot bootloader for USB

{% include custom/mcu/stm32f4/canboot_compile_usb_deployer.html %}

{% include custom/mcu/stm32f4/canboot_flash_deployer.html %}

{% include custom/mcu/super8/fly_super8_links.html %}

