---
title: Fly-E3-Pro-V3 CanBoot bootloader for USB
tags: []
keywords: 
last_updated: 11/07/2023
summary: "Fly E3 pro v3 CanBoot bootloader for USB"
sidebar: mydoc_sidebar
permalink: fly-e3_pro_v3_canboot_usb.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly E3 Pro v3
firmware: usb
ver: "V3" 


com: "USB on PA11/PA12"

cancom_img1: "fly-super8/fly-super8_canboot_menuconfig_usb.png"
cancom_cap1: "CanBoot Menu Config USB"

cancom_img2: "fly-e3_v2/fly-e3_v2_sd_card.png"
cancom_cap2: "Fly E3 v2 SD card"

cancom_img3: "fly-e3_v2/fly-e3_v2_reset.png"
cancom_cap3: "Fly E3 v2 reset button"

canburn_img1: "fly-super8/fly-super8_pro_klipper_flash_fw_serial_usb.png"
canburn_cap1: "Fly E3 v2 dfu lsusb"

canburn_img2: "fly-super8/fly-super8_canbus_usb_flash.png"
canburn_cap2: "Fly E3 v2 burn result"

---

## Configuring and installing CanBoot bootloader for USB

{% include custom/mcu/stm32f4/canboot_compile_usb_deployer.html %}

{% include custom/mcu/stm32f4/canboot_flash_deployer.html %}

{% include custom/can/sht_links.html %}

