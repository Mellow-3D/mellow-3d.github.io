---
title: Fly Gemini V3 MCU Klipper USB firmware
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly Gemini V3 Klipper host"
sidebar: mydoc_sidebar
permalink: fly-gemini_v3_klipper_mcu_usb.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly Gemini V3
firmware: usb
version: v1


com: "USB on PA11/PA12"


klipcom_img1: "fly-gemini-v2/fly_gemini_klipper_menuconfig_usb.png"
klipcom_cap1: "Klipper Menu Config USB"

klipcom_img2: "fly-gemini-v2/fly_gemini_klipper_usb_burn.png"
klipcom_cap2: "Burn Klipper firmware over USB"

klipcom_img3: "fly-gemini-v2/flash-can_query.png"
klipcom_cap3: "Flash Can Query"


---

## Configuring and installing Klipper for USB

{% include custom/sbc/fly-gemini_v3_klipper_compile.html %}

{% include custom/can/sht_links.html %}