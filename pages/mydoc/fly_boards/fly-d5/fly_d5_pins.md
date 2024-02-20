---
title: Fly-D5 Pin Names
tags: []
keywords: 
last_updated: 20/02/2024
summary: "The pin names of the Fly-D5"
sidebar: mydoc_sidebar
permalink: fly_d5_pins.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: Fly-D5
version: v2

mcu: "fly-d5"

img1: "fly-d5/Fly-D5-Pinout.svg"
cap1: "Fly-D5 Pin Diagram"
---

    {% capture boardname %}{{ page.boardname }}{% endcapture %}

    {% capture mcu %}{{ page.mcu }}{% endcapture %}

    {% capture img1 %}{{page.img1 }}{% endcapture %}
    {% capture cap1 %}{{page.cap1 }}{% endcapture %}
    {% capture url1 %} .\images\{{ page.img1 }} {% endcapture %}

## Fly-D5 Pinout Diagram

{%
include image.html
file=img1
url=url1
alt=cap1
caption=cap1
%}
