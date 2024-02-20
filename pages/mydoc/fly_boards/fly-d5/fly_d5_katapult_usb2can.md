---
title: Katapult Configuration for the Fly-D5 on USB to CAN Bridge Mode
tags: []
keywords: 
last_updated: 19/02/2024
summary: "How to Configure Katapult for USB to CAN Bridge Operation on the Fly-D5"
sidebar: mydoc_sidebar
permalink: fly_d5_katapult_usb2can.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-D5
firmware: USB
mcu: "STM32"
kconfig_name: d5
architecture: "(STMicroelectronics STM32)"
processor: "(STM32F072)"
deployment: "(8KiB bootloader)"
clock: "(8 MHz crystal)"
communication: "(USB (on PA11/PA12))"
application_offset: "(8KiB offset)"
gpio_bootloader_set: "()"
support_bootloader_entry: "[*]"
enable_bootloader_gpio: "[&nbsp;]"
enable_status: "[&nbsp;]"
board_type: "mainboard"
katapult_file: "katapult.bin"

katapult_img1: "katapult/stm32f072_usb_deployer.png"
katapult_cap1: "Katapult Menu Config USB"

katapult_img2: "dfu/stm32_dfu.png"
katapult_cap2: "STM32 DFU Mode Detected"

katapult_img3: "dfu/stm32_dfu_flash.png"
katapult_cap3: "DFU Mode Flash Successful"

installKlipperURL: "./fly_d5_klipper_usb2can.html"
installKlipperName: "Klipper for USB to CAN Bridge configuration section"
---

## Configuring and installing Katapult bootloader for USB to CAN Bridge Mode

{% include custom/katapult/compile.html %}

{% include custom/katapult/flash_dfu.html %}

{% include custom/mcu/d5/fly_d5_links.html %}
