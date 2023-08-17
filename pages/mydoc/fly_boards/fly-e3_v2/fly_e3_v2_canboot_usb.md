---
title: Katapult Configuration for the Fly-E3-v2 on USB
tags: []
keywords: 
last_updated: 16/08/2023
summary: "How to Configure Katapult for USB Operation on the Fly-E3-v2"
sidebar: mydoc_sidebar
permalink: fly_e3_v2_canboot_usb.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-E3-v2
firmware: USB
mcu: "STM32"
kconfig_name: e3v2
architecture: "STMicroelectronics STM32"
processor: "STM32F407"
deployment: "32KiB bootloader"
clock: "8 MHz crystal"
communication: "USB (on PA11/PA12)"
application_offset: "32KiB offset"
gpio_bootloader_set: ""
support_bootloader_entry: "*"
enable_bootloader_gpio: ""
enable_status: "*"
board_type: "mainboard"
katapult_file: "deployer.bin"

katapult_img1: "katapult/stm32f407_usb_deployer.png"
katapult_cap1: "Katapult Menu Config USB"

katapult_img2: "fly-e3_v2/fly-e3_v2_sd_card.png"
katapult_cap2: "Fly-E3-v2 SD card"

katapult_img3: "fly-e3_v2/fly-e3_v2_reset.png"
katapult_cap3: "Fly-E3-v2 reset button"

installKlipperURL: "./fly_e3_v2_klipper_usb.html"
installKlipperName: "Klipper for USB configuration section"
---

## Configuring and installing CanBoot bootloader for USB

{% include custom/katapult/compile.html %}

{% include custom/katapult/flash_deployer.html %}

{% include custom/mcu/e3v2/fly_e3_v2_links.html %}
