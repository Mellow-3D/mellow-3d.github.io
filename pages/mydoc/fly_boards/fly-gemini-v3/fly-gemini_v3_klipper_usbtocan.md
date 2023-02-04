---
title: Fly-Gemini v3 Klipper firmware in USB to Can Bridge
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-Gemini v3 Klipper USB to CAN"
sidebar: mydoc_sidebar
permalink: fly-gemini_v3_klipper_usbtocan.html
folder: mydoc
comments: false
toc: true
datatable: true


micro: "STMicroelectronics STM32"
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"
com: "USB to CAN Bridge on PA11/PA12"
appoffset: "32 KiB offset"
canspeed: ""


klipcom_img1: "fly-super8/fly-super8_klipper_menuconfig_usb_can_bridge.png"
klipcom_cap1: "Klipper Menu Config USB to CAN"

klipcom_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipcom_cap2: "Burn Klipper firmware over USB"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"


---

## Configuring and installing Klipper for USB to CAN bridge mode


{% include custom/sbc/fly-gemini_v3_klipper_compile.html %}

{% include custom/can/sht_links.html %}