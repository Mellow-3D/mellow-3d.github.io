---
title: Fly-Super8 CanBoot bootloader for CANbus
tags: []
keywords: 
last_updated: 16/07/2023
summary: "Fly-Super8 CanBoot bootloader for CANbus"
sidebar: mydoc_sidebar
permalink: fly_super8_canboot_can.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-Super8
firmware: can
ver: "V 1.2" 

micro: "STMicroelectronics STM32"
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"
com: "CAN bus on PB8/PB9"
appoffset: "32 KiB offset"
canspeed: "500000"

klipperurl: "[Klipper for CAN bus configuration section](fly_super8_klipper_can.html)"

cancom_img1: "fly-super8/fly-super8_canboot_menuconfig_can.png"
cancom_cap1: "CanBoot Menuconfig"

cancom_img2: "fly-super8/fly-super8_sd.png"
cancom_cap2: "Fly-Super8 SD card slot"

cancom_img3: "fly-super8/fly-super8_reset.png"
cancom_cap3: "Fly-Super8 Reset button"

canburn_img1: "fly-super8/fly-super8_pro_klipper_flash_fw_serial_usb.png"
canburn_cap1: "Fly-Super8 dfu lsusb"

canburn_img2: "fly-super8/fly-super8_canbus_usb_flash.png"
canburn_cap2: "Fly-Super8 burn result"

installKlipperURL: "./fly_super8_klipper_can.html"
installKlipperName: "Klipper for CANbus configuration section"

---

## Configuring and installing CanBoot bootloader for CANbus

{% include custom/mcu/stm32f4/canboot_compile_can_deployer.html %}

{% include custom/mcu/stm32f4/canboot_flash_deployer.html %}

{% include custom/mcu/super8/fly_super8_links.html %}

