---
title: Fly-E3-Pro-V3 CanBoot bootloader for USB
tags: []
keywords: 
last_updated: 17/02/2024
summary: "How to compile and install the CanBoot bootloader for USB operation on the Fly-E3-Pro-V3"
sidebar: mydoc_sidebar
permalink: fly_e3_pro_v3_katapult_usb.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-E3-Pro-V3
firmware: USB
mcu: "STM32"
kconfig_name: e3prov3
architecture: "(STMicroelectronics STM32)"
processor: "(STM32F407)"
deployment: "(32KiB bootloader)"
clock: "(8 MHz crystal)"
communication: "(USB (on PA11/PA12))"
application_offset: "(32KiB offset)"
gpio_bootloader_set: "()"
support_bootloader_entry: "[*]"
enable_bootloader_gpio: "[&nbsp;]"
enable_status: "[&nbsp;]"
board_type: "mainboard"
katapult_file: "deployer.bin"

katapult_img1: "katapult/stm32f407_usb_deployer.png"
katapult_cap1: "Katapult Menu Config USB"

katapult_img2: "fly-e3_v2/fly-e3_v2_sd_card.png"
katapult_cap2: "Fly-E3-Pro-V3 SD card"

katapult_img3: "fly-e3_v2/fly-e3_v2_reset.png"
katapult_cap3: "Fly-E3-Pro-V3 reset button"

installKlipperURL: "./fly_e3_pro_v3_klipper_usb.html"
installKlipperName: "Klipper for USB configuration section"
---

## Configuring and installing CanBoot bootloader for USB

{% include custom/katapult/compile.html %}

{% include custom/katapult/flash_deployer.html %}

{% include custom/mcu/e3prov3/fly_e3_pro_v3_links.html %}
