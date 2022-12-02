---
title: Fly Pi General Information
tags: []
keywords: 
last_updated: 20/10/2022
summary: "General information regarding the Fly Pi"
sidebar: mydoc_sidebar
permalink: fly_pi_general.html
folder: mydoc
comments: false
toc: false
datatable: true

fly_pi_img1: "fly-pi/fly_pi_general.webp"
fly_pi_cap1: "Fly Pi Overview"

---

    {% capture mcu %}{{ page.mcu }}{% endcapture %}

    {% capture mcufile %}{{ page.mcufile }}{% endcapture %}

    {% capture fly_pi_img1 %}{{page.fly_pi_img1 }}{% endcapture %}
    {% capture fly_pi_cap1 %}{{page.fly_pi_cap1 }}{% endcapture %}
    {% capture fly_pi_url1 %} .\images\{{ page.fly_pi_img1 }} {% endcapture %}

## Overview

This page covers any general information for the Fly-Pi board.  
It is currently available through [AliExpress](https://www.aliexpress.us/item/3256804173218933.html). 

{% 
include image.html 
file=fly_pi_img1
url=fly_pi_url1
alt=fly_pi_cap1
caption=fly_pi_cap1
%}

### Maximum Input voltage

#### Board/Bed Power

The board power input can handle voltage up to 24v.

### Initial Installation

The board that you will receive doesn't have any firmware installed so when plugged into a computer, the board will show as an unidentified device.
Follow the [SD card instructions](fly-pi_sd_card.html) to build an SD card with Fly OS. If you have purchased the optional [M2WE 16G eMMC & 5G Wifi board](https://www.aliexpress.us/item/3256804602300590.html) it will come with the FLY OS pre installed on the M2WE.  

{% include custom/can/sht_links.html %}
