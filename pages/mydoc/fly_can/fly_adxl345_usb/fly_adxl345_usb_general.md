---

title: Fly-ADXL345-USB General Information
tags: []
keywords: 
last_updated: 21/08/2023
summary: "General information regarding the Fly-ADXL345-USB"
sidebar: mydoc_sidebar
permalink: fly_adxl345_usb_general.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: Fly-ADXL345-USB

overview_img1: "fly_adxl345_usb/overview.png"
overview_cap1: "Fly-ADXL345-USB Front and Rear view"

overview_img2: "fly_adxl345_usb/size.png"
overview_cap2: "Fly-ADXL345-USB dimensions"

---
## {{ page.boardname }} Overview

    {% capture mcustep %}{{ page.mcustep }}{% endcapture %}
    {% capture mcustep2 %}{{ page.mcustep2 }}{% endcapture %}
    {% capture mcusch %}{{ page.mcusch }}{% endcapture %}

    {% capture overurl1 %}.\images\{{page.overview_img1}}{% endcapture %}
    {% capture overurl2 %}.\images\{{page.overview_img2}}{% endcapture %}       
    {% capture overurl3 %}.\images\{{page.overview_img3}}{% endcapture %}   

### Description

The {{page.boardname}} uses USB communication to connect the host computer and features an onboard ADXL345 accelerometer to measure resonance for input shaper.  
The {{page.boardname}} can be purchased from [AliExpress](https://s.click.aliexpress.com/e/_DmBXwpZ)

{% include image.html file=page.overview_img1 url=overurl1 alt=page.overview_cap1 caption=page.overview_cap1 %}

{% include image.html file=page.overview_img2 url=overurl2 alt=page.overview_cap2 caption=page.overview_cap2 %}

{% include custom/mcu/adxl345_usb/adxl345_usb_links.html %}
