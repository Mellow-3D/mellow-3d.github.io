---
title: Fly-407ZG CanBoot bootloader for USB
tags: []
keywords: 
last_updated: 19/07/2023
summary: "How to compile and install the CanBoot bootloader for USB operation on the Fly-407ZG"
sidebar: mydoc_sidebar
permalink: fly_407zg_canboot_usb.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-407ZG
firmware: usb
ver: "" 
processor: "STM32F407"
com: "USB (on PA11/PA12)"
micro: "STMicroelectronics STM32"
offset: "32KiB bootloader"
clock: "8 MHz crystal"
appoffset: "32KiB offset"

klipperurl: "[Klipper for USB configuration section](fly-407zg_klipper_usb.html)"

klipperurl2: ""

cancom_img1: "fly-super8/fly-super8_canboot_menuconfig_usb.png"
cancom_cap1: "CanBoot Menuconfig"

cancom_img2: "fly-407zg/fly-f407zg_sdcard.png"
cancom_cap2: "Fly-407ZG SD card slot"

cancom_img3: "fly-407zg/fly-f407zg_reset.png"
cancom_cap3: "Fly-407ZG Reset button"

installKlipperURL: "./fly_407zg_klipper_usb.html"
installKlipperName: "Klipper for USB configuration section"
---

## Configuring and installing CanBoot bootloader for USB

{% include custom/mcu/stm32f4/canboot_compile_usb_deployer.html %}

{% include custom/mcu/stm32f4/canboot_flash_deployer.html %}

{% include custom/mcu/407zg/fly_407zg_links.html %}

