---
title: Fly-E3v2 Klipper firmware in USB to Can Bridge Mode
tags: []
keywords: 
last_updated: 15/07/2023
summary: "Fly-E3-v2 Klipper USB to CAN Bridge Mode"
sidebar: mydoc_sidebar
permalink: fly_e3_v2_klipper_usb2can.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-E3-v2
firmware: usbtocan
version: v1
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"
micro: "STMicroelectronics STM32"
com: "USB to CAN bus bridge (USB on PA11/PA12)"
canspeed: "500000"
caninterface: "CAN bus (on PB8/PB9)"

klipcom_img1: "fly-super8/fly-super8_klipper_menuconfig_usb_can_bridge.png"
klipcom_cap1: "Klipper Menu Config USB to CAN"

klipcom_img2: "fly-super8/fly-super8_klipper_usb_burn.png"
klipcom_cap2: "Burn Klipper firmware over USB"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"

kconfig_name: "e3v2"
---

## Configuring and installing Klipper for USB to CAN bridge mode

{% include tip.html content="To read more about the KCONFIG_CONFIG option, see [here](https://docs.vorondesign.com/community/howto/drachenkatze/automating_klipper_mcu_updates.html)" %}

{% include note.html content="If you are planning to use CANBoot bootloader with Klipper in USB to CAN bridge mode you will want to configure [CanBoot in USB mode](./fly_e3_v2_canboot_usb.html)" %}

{% include custom/mcu/stm32f4/klipper_menuconfig_usb2can.html %}

{% include custom/mcu/stm32f4/klipper_flash_canboot_usb2can.html %}

{% include custom/mcu/e3v2/fly_e3_v2_links.html %}