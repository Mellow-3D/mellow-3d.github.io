---
title: Fly Mini 12864 Pin diagram
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly Mini 12864 Display pin diagram"
sidebar: mydoc_sidebar
permalink: fly_mini12864_pins.html
folder: mydoc
comments: false
toc: false
datatable: true

boardname: "Fly-Mini 12864"
aliexpress: "[Mellow store on Aliexpress](https://www.aliexpress.us/item/3256803392961881.html)"

display_img1: "fly-mini12864/fly-mini12864_pins.png"
display_cap1: "Fly-Mini 12864"

---

    {% capture boardname %}{{ page.boardname }}{% endcapture %}
    {% capture aliexpress %}{{ page.aliexpress }}{% endcapture %}

    {% capture display_img1 %}{{page.display_img1}}{% endcapture %}
    {% capture display_cap1 %}{{page.display_cap1}}{% endcapture %}
    {% capture display_url1 %}.\images\{{page.display_img1}}{% endcapture %}  



## Pin Diagram
{{boardname}} Display

{% 
include image.html 
file=display_img1
url=display_url1 
alt=display_cap1
caption=display_cap1
%}

### EXP1

<div class="datatable-begin"></div>

|Socket|Pin Number|Pin Name 1|Pin Name 2|Alias|Note|
| :------------- |:-------------|:-------------|:-------------|:-------------|:-------------|
|EXP1|1|5v|VCC|EXP1_10||
|EXP1|2|GND|GND|EXP1_9||
|EXP1|3|LCD_D7|Blue|EXP1_8||
|EXP1|4|LCD_D6|Green|EXP1_7||
|EXP1|5|LCD_D5|Red|EXP1_6|Neopixel Pin|
|EXP1|6|LCD_D4|LCD_RST|EXP1_5||
|EXP1|7|LCD_RS|LCD_A0|EXP1_4||
|EXP1|8|LCD_EN|LCD_CS|EXP1_3||
|EXP1|9|LCD_BTN_ENC|BTN_ENC|EXP1_2||
|EXP1|10|BEEP|BEEP|EXP1_1||

<div class="datatable-end"></div>

### EXP2

<div class="datatable-begin"></div>

|Socket|Pin Number|Pin Name 1|Pin Name 2|Alias|Note|
| :------------- |:-------------|:-------------|:-------------|:-------------|:-------------|
|EXP2|1|KILL|KILL|EXP2_10||
|EXP2|2|GND|GND|EXP2_9||
|EXP2|3|RST|RST|EXP2_8||
|EXP2|4|LCD_CD|CD|EXP2_7||
|EXP2|5|LCD_MOSI|MOSI|EXP2_6||
|EXP2|6|LCD_BTN_EN2|BTN_EN2|EXP2_5||
|EXP2|7|LCD_SS|SS|EXP2_4||
|EXP2|8|LCD_BTN_EN1|BTN_EN1|EXP2_3||
|EXP2|9|LCD_SCK|SCK|EXP2_2||
|EXP2|10|LCD_MISO|MISO|EXP2_1||

<div class="datatable-end"></div>

