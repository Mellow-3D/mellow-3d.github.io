---
title: Configuring the Mellow SHT-42 canbus tool boards for Klipper on USB
tags: [content_types]
keywords: 
last_updated: 20/10/2022
summary: "Klipper Configuration for the Fly SHT-42 on USB"
sidebar: mydoc_sidebar
permalink: fly-sht42_klipper_usb.html
folder: mydoc
comments: false
toc: false
datatable: true
boardname: sht42
firmware: usb
---

{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}


* TOC
{:toc}

## Setup steps

### Toolboard firmware

{% include custom/can/sht_canboot_compile.html %}

{% include custom/can/sht_canboot_burn.html %}

{% include custom/can/sht_klipper_compile.html %}

{% include custom/can/sht_klipper_configure.html %}