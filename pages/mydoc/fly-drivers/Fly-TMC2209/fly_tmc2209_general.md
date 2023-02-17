---
title: Fly TMC2209 Stepstick
tags: []
keywords: 
last_updated: 20/10/2022
summary: "General information regarding the Fly TMC2209"
sidebar: mydoc_sidebar
permalink: fly_tmc2209_general.html
folder: mydoc
comments: false
toc: true
datatable: true
driver_img1: "fly-2209/fly-2209_general.webp"
driver_cap1: "Fly-TMC2209 Overview"

driver_img2: "fly-2209/fly-2209_dimensions.webp"
driver_cap2: "Fly-TMC2209 Dimensions"

driver_img3: "fly-2209/fly-2209_pins.webp"
driver_cap3: "Fly-TMC2209 pin map"

driver_img4: "fly-2209/fly-2209_diag.webp"
driver_cap4: "Fly-TMC2209 Diag switch"

driver_img5: "fly-2209/fly-2209_uart.webp"
driver_cap5: "Fly-TMC2209 UART resistor"

---

    {% capture driver_img1 %}{{page.driver_img1 }}{% endcapture %}
    {% capture driver_cap1 %}{{page.driver_cap1 }}{% endcapture %}
    {% capture driver_url1 %} .\images\{{ page.driver_img1 }} {% endcapture %}

    {% capture driver_img2 %}{{page.driver_img2 }}{% endcapture %}
    {% capture driver_cap2 %}{{page.driver_cap2 }}{% endcapture %}
    {% capture driver_url2 %} .\images\{{ page.driver_img2 }} {% endcapture %}

    {% capture driver_img3 %}{{page.driver_img3 }}{% endcapture %}
    {% capture driver_cap3 %}{{page.driver_cap3 }}{% endcapture %}
    {% capture driver_url3 %} .\images\{{ page.driver_img3 }} {% endcapture %}

    {% capture driver_img4 %}{{page.driver_img4 }}{% endcapture %}
    {% capture driver_cap4 %}{{page.driver_cap4 }}{% endcapture %}
    {% capture driver_url4 %} .\images\{{ page.driver_img4 }} {% endcapture %}

    {% capture driver_img5 %}{{page.driver_img5 }}{% endcapture %}
    {% capture driver_cap5 %}{{page.driver_cap5 }}{% endcapture %}
    {% capture driver_url5 %} .\images\{{ page.driver_img5 }} {% endcapture %}

## Overview 

### Fly TMC2209 Driver

  {% 
  include image.html 
  file=driver_img1
  url=driver_url1
  alt=driver_cap1
  caption=driver_cap1
  %}

### Dimensions

  {% 
  include image.html 
  file=driver_img2
  url=driver_url2
  alt=driver_cap2
  caption=driver_cap2
  %}

### Circuit Diagram
  {% 
  include image.html 
  file=driver_img3
  url=driver_url3
  alt=driver_cap3
  caption=driver_cap3
  %}

### Diag switch
  {% 
  include image.html 
  file=driver_img4
  url=driver_url4
  alt=driver_cap4
  caption=driver_cap4
  %}

### UART
  {% 
  include image.html 
  file=driver_img5
  url=driver_url5
  alt=driver_cap5
  caption=driver_cap5
  %}
