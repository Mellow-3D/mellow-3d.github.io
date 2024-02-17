---
title: Klipper Configuration for the Fly-ERCF-Easy-BRD-V1.1 on CANbus
tags: []
keywords: 
last_updated: 04/09/2023
summary: "Klipper Configuration for the Fly-ERCF-Easy-BRD-V1.1 on CANbus"
sidebar: mydoc_sidebar
permalink: fly_ercf_v1.1_klipper_can_updating.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: Fly-ERCF-Easy-BRD-V1.1
firmware: CANbus
mcu: "rp2040"
version: v1
kconfig_name: ercfv1.1
low_level: "[*]"
architecture: "(Raspberry Pi RP2040)"
bootloader_offset: "(16KiB bootloader)"
communication: "(CAN bus)"
can_rx: "(4)"
can_tx: "(5)"
can_bus_speed: "(1000000)"
gpio_startup: "(gpio24)"
board_type: "toolboard"
klipper_file: "klipper.uf2"
120rurl: "./fly_ercf_v1.1_120r.html"
state: "update"

klipper_img1: "klipper/rp2040_can_gpio17.png"
klipper_cap1: "Klipper Menu Config CAN"

klipper_img2: "fly-super8/flash-can_query.png"
klipper_cap2: "Flash Can Query"

klipper_img3: "fly-super8/fly-super8_klipper_canboot_burn.png"
klipper_cap3: "Burn Klipper firmware over CANbus"

---

{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}

{% include custom/klipper/menuconfig.html %}

{% include custom/klipper/flash_katapult_can.html %}

{% include custom/mcu/ercf_v1.1/ercf_v1.1_links.html %}
