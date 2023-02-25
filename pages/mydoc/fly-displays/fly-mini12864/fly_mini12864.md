---
title: Fly Mini 12864 display General Information
tags: []
keywords: 
last_updated: 20/10/2022
summary: "General information regarding the Fly Mini 12864 Display"
sidebar: mydoc_sidebar
permalink: fly_mini12864_general.html
folder: mydoc
comments: false
toc: false
datatable: true

boardname: "Fly-Mini 12864"
aliexpress: "[Mellow store on Aliexpress](https://www.aliexpress.us/item/3256803392961881.html)"

display_img1: "fly-mini12864/fly-mini12864_front.png"
display_cap1: "Fly-Mini 12864"

display_img2: "fly-mini12864/fly-mini12864_dimensions.jpg"
display_cap2: "Fly-Mini 12864 Dimensions"

---

    {% capture boardname %}{{ page.boardname }}{% endcapture %}
    {% capture aliexpress %}{{ page.aliexpress }}{% endcapture %}

    {% capture display_img1 %}{{page.display_img1}}{% endcapture %}
    {% capture display_cap1 %}{{page.display_cap1}}{% endcapture %}
    {% capture display_url1 %}.\images\{{page.display_img1}}{% endcapture %}  

    {% capture display_img2 %}{{page.display_img2}}{% endcapture %}
    {% capture display_cap2 %}{{page.display_cap2}}{% endcapture %}
    {% capture display_url2 %}.\images\{{page.display_img2}}{% endcapture %}  


## Overview 
{{boardname}} Display

{% 
include image.html 
file=display_img1
url=display_url1 
alt=display_cap1
caption=display_cap1
%}

Avaliable from the {{aliexpress}}

### General Information

 - Model Number : FLY Mini 12864 V1.0
 - Power input: DC5v
 - SD Card logic voltage: 3.3V/5V
 - 3 addressable WS2182 RGB LEDs for the display and knob. 
 - SupperSupported firmware: Marlin, Reprap(Duet), and Klipper 
 - Connects through EXP1 and EXP2 ports on the MCU.


### Dimensions

{% 
include image.html 
file=display_img2
url=display_url2
alt=display_cap2
caption=display_cap2
%}

 - Size: 104.99*47MM

### Supported Mellow boards

 - [Fly CDY V3](./fly-cdy_v3.html)
 - [Fly E3 V2](./fly-e3_v2.html)
 - [Fly E3 Pro](./fly-e3_pro_v3.html)
 - [Fly Super 8](./fly-super8_general.html)
 - [Fly Super 8 Pro](./fly-super8_pro_general.html)
 - [Fly 407ZG](./fly_407zg.html)
 - [Fly Gemini V2](fly-gemini_v2_general.html)
 - [Fly Gemini V3](fly-gemini_v3_general.html)