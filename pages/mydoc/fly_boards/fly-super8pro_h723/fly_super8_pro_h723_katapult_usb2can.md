---
title: Fly-Super8Pro H723 CanBoot bootloader for USB to CAN bridge mode
tags: []
keywords: 
last_updated: 18/02/2024
summary: "Fly-Super8Pro H723 CanBoot Pro bootloader for USB to CAN bridge"
sidebar: mydoc_sidebar
permalink: fly-super8_pro_h723_canboot_usb2can.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-Super8Pro
firmware: USB
mcu: "STM32"
kconfig_name: super8proh723
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

katapult_img2: "fly-super8_pro/fly_super8pro_sd_card.png"
katapult_cap2: "Fly-Super8Pro SD card"

katapult_img3: "fly-super8_pro/fly_super8pro_reset.png"
katapult_cap3: "Fly-Super8Pro reset button"

installKlipperURL: "./fly_super8_pro_klipper_usb2can.html"
installKlipperName: "Klipper for USB to CAN Bridge mode configuration section"
---

## Configuring and installing Katapult bootloader for USB to CAN Bridge Mode

{% include custom/katapult/compile.html %}

## USB Power Jumper

Add a jumper as shown below to ensure the board can be powered from USB power.  

{% include image.html file="fly-super8_pro/fly_super8pro_usb_power.png" alt="Fly-Super8Pro H723 USB Power Jumper" caption="Fly-Super8Pro H723 USB Power Jumper" %}

{% include custom/katapult/flash_deployer.html %}

{% include custom/mcu/super8/fly_super8pro_links.html %}
