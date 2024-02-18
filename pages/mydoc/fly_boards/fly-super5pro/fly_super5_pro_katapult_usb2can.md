---
title: Katapult Configuration for the Fly-Super5Pro on USB to CAN Bridge Mode
tags: []
keywords: 
last_updated: 18/02/2024
summary: "How to Configure Katapult for USB to CAN Bridge Operation on the Fly-Super5Pro"
sidebar: mydoc_sidebar
permalink: fly_super5_pro_katapult_usb2can.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-Super5Pro
firmware: USB
mcu: "STM32"
kconfig_name: super5pro
architecture: "(STMicroelectronics STM32)"
processor: "(STM32H723)"
deployment: "(128KiB bootloader (SKR SE BX v2.0))"
clock: "(25 MHz crystal)"
communication: "(USB (on PA11/PA12))"
application_offset: "(128KiB offset)"
gpio_bootloader_set: "()"
support_bootloader_entry: "[*]"
enable_bootloader_gpio: "[&nbsp;]"
enable_status: "[&nbsp;]"
board_type: "mainboard"
katapult_file: "deployer.bin"

katapult_img1: "katapult/stm32h723_usb_deployer.png"
katapult_cap1: "Katapult Menu Config CAN"

katapult_img2: "fly-super5_pro/fly_super5pro_sd_card.png"
katapult_cap2: "Fly-Super5Pro SD card"

katapult_img3: "fly-super5_pro/fly_super5pro_reset.png"
katapult_cap3: "Fly-Super5Pro reset button"

installKlipperURL: "./fly_super5_pro_klipper_usb2can.html"
installKlipperName: "Klipper for USB to CAN Bridge mode configuration section"
---

## Configuring and installing Katapult bootloader for USB to CAN Bridge Mode

{% include custom/katapult/compile.html %}

{% include custom/katapult/flash_deployer.html %}

{% include custom/mcu/super5_pro/fly_super5pro_links.html %}
