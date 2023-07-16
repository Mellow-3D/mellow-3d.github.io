---
title: Updating Klipper Firmware on a Fly-Super8 in USB to CAN Bridge mode
tags: []
keywords: 
last_updated: 16/07/2023
summary: "How to update the klipper firmware running on a Fly-Super8 in USB to CAN Bridge mode"
sidebar: mydoc_sidebar
permalink: fly_super8_klipper_usb2can_updating.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-Super 8
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

klipcom_img2: "fly-super8/fly-super8_klipper_makeflash_burn.png"
klipcom_cap2: "Burn Klipper firmware over USB"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"

kconfig_name: "super8"
---

## Configuring and installing Klipper for USB to CAN bridge mode

{% include warning.html content="Super 8 Version 1.0 does not support USB to CAN bridge mode." %}

{% include tip.html content="To read more about the KCONFIG_CONFIG option, see [here](https://docs.vorondesign.com/community/howto/drachenkatze/automating_klipper_mcu_updates.html)" %}

{% include note.html content="If you are planning to use CANBoot bootloader with Klipper in USB to CAN bridge mode you will want to configure [CanBoot in USB mode](./fly_super8_canboot_usb.html)" %}

{% include custom/mcu/stm32f4/klipper_menuconfig_usb2can_updating.html %}

{% include custom/mcu/stm32f4/klipper_flash_canboot_usb2can_updating.html %}

{% include custom/mcu/super8/fly_super8_links.html %}