---
title: Fly-DP5 Pin Names
tags: []
keywords: 
last_updated: 02/03/2024
summary: "The pin names of the Fly-DP5"
sidebar: mydoc_sidebar
permalink: fly_dp5_pins.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-DP5
version: v2

mcu: "fly-dp5"

img1: "fly-dp5/Fly-DP5-Pinout.svg"
cap1: "Fly-DP5 Pin Diagram"
---

    {% capture boardname %}{{ page.boardname }}{% endcapture %}

    {% capture mcu %}{{ page.mcu }}{% endcapture %}

    {% capture img1 %}{{page.img1 }}{% endcapture %}
    {% capture cap1 %}{{page.cap1 }}{% endcapture %}
    {% capture url1 %} .\images\{{ page.img1 }} {% endcapture %}

## Fly-DP5 Pinout Diagram

{%
include image.html
file=img1
url=url1
alt=cap1
caption=cap1
%}
