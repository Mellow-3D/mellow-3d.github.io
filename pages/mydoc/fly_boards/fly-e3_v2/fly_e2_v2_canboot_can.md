---
title: Fly-E3-v2 CanBoot bootloader for CAN bus
tags: []
keywords: 
last_updated: 04/09/2023
summary: "Fly-E3-v2 CanBoot bootloader for CAN bus"
sidebar: mydoc_sidebar
permalink: fly_e3_v2_canboot_can.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-E3-v2
firmware: CANbus
mcu: "STM32"
version: v1
kconfig_name: e3v2
architecture: "(STMicroelectronics STM32)"
processor: "(STM32F407)"
deployment: "(32KiB bootloader)"
clock: "(8 MHz crystal)"
communication: "(CAN bus (on PB8/PB9))"
application_offset: "(32KiB offset)"
can_bus_speed: "(1000000)"
gpio_bootloader_set: "()"
support_bootloader_entry: "[*]"
enable_bootloader_gpio: "[&nbsp;]"
enable_status: "[&nbsp;]"
board_type: "mainboard"
katapult_file: "deployer.bin"

katapult_img1: "katapult/stm32f407_can_deployer_pb8pb9.png"
katapult_cap1: "Katapult Menu Config CAN"

katapult_img2: "fly-e3_v2/fly-e3_v2_sd_card.png"
katapult_cap2: "Fly-E3-v2 SD card"

katapult_img3: "fly-e3_v2/fly-e3_v2_reset.png"
katapult_cap3: "Fly-E3-v2 reset button"

installKlipperURL: "./fly_e3_v2_klipper_can.html"
installKlipperName: "Klipper for CANbus configuration section"

---

## Configuring and installing CanBoot bootloader for CAN bus

{% include custom/katapult/compile.html %}

{% include custom/katapult/flash_deployer.html %}

{% include custom/mcu/e3v2/fly_e3_v2_links.html %}
