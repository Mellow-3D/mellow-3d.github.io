---
title: Fly Mini 12864 display Klipper configuration
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Klipper COnfiguration for the Fly Mini 12864 Display"
sidebar: mydoc_sidebar
permalink: fly_mini12864_klipper.html
folder: mydoc
comments: false
toc: true
datatable: true

boardname: "Fly-Mini 12864"
aliexpress: "[Mellow store on Aliexpress](https://www.aliexpress.us/item/3256803392961881.html)"



---

        {% capture boardname %}{{ page.boardname }}{% endcapture %}

## {{boardname}} Klipper Configuration

## Display Configuration
 - Add to klipper printer.cfg
```
[display]
lcd_type: uc1701
cs_pin: EXP1_3
a0_pin: EXP1_4
rst_pin: EXP1_5
contrast: 63
encoder_pins: ^EXP2_5, ^!EXP2_3
click_pin: ^!EXP1_2
```

## Neopixel Configuration
 - Add to klipper printer.cfg
 ```
[neopixel fly_mini12864]
pin: EXP1_6
chain_count: 3
initial_RED: 0.1
initial_GREEN: 0.5
initial_BLUE: 0.0
color_order: RGB
```

## Mellow Board Alias file settings for the {{boardname}}

### Fly CDY V3

 - Main page for the [Fly CDY V3](./fly-cdy_v3.html)
 - [Download a copy of the Fly CDY V3 aliases file](./files/fly-cdy_v3/FLY-CDY_V3.cfg)

```
    # EXP1 header
    EXP1_1=<NC>>,  EXP1_3=PB2,  EXP1_5=PE15,   EXP1_7=PA13,  EXP1_9=<GND>,
    EXP1_2=PA9,  EXP1_4=PA10,  EXP1_6=PE14,   EXP1_8=PA14,  EXP1_10=<5V>,
    # EXP2 header
    EXP2_1=PA6, EXP2_3=PD8,  EXP2_5=PD9,  EXP2_7=PC13,   EXP2_9=<GND>,
    EXP2_2=PA5, EXP2_4=PA4,  EXP2_6=PA7,  EXP2_8=<RST>, EXP2_10=<5V>,
```

### Fly E3 V2

 - Main page for the [Fly E3 V2](./fly-e3_v2.html)
- [Download a copy of the Fly E2 V2 aliases file](./files/fly-e3_v2/FLY_E3_V2.cfg)

```
    # EXP1 header
    EXP1_1=PD10,  EXP1_3=PA8,  EXP1_5=PE14,   EXP1_7=PA14,  EXP1_9=<GND>,
    EXP1_2=PA9,  EXP1_4=PA10,  EXP1_6=PE15,   EXP1_8=A13,  EXP1_10=<5V>,
    # EXP2 header
    EXP2_1=PA6, EXP2_3=PB11,  EXP2_5=PB10,  EXP2_7=PE13,   EXP2_9=<GND>,
    EXP2_2=PA5, EXP2_4=PA4,  EXP2_6=PA7,  EXP2_8=<NC>, EXP2_10=<NC>,
```

### Fly E3 Pro V3

 - Main page for the [Fly E3 Pro V3](./fly-e3_pro_v3.html)
- [Download a copy of the Fly E3 Pro V3 aliases file](./files/fly-e3_pro_v3/FLY_E3_pro_V3.cfg)

```
    # EXP1 header
    EXP1_1=PE11, EXP1_3=PA14,  EXP1_5=PE9,   EXP1_7=PE7,  EXP1_9=<GND>,
    EXP1_2=PE12,  EXP1_4=PE6,  EXP1_6=PE10,   EXP1_8=PE8,  EXP1_10=<5V>,
    # EXP2 header
    EXP2_1=PB4, EXP2_3=PA10,  EXP2_5=PA9,  EXP2_7=PA13,   EXP2_9=<GND>,
    EXP2_2=PB3, EXP2_4=PB2,  EXP2_6=PB5,  EXP2_8=<RST>, EXP2_10=<NC>,
```


### Fly Super 8

 - Main page for the [Fly Super 8](./fly-super8_general.html)
- [Download a copy of the Super 8 aliases file](./files/super8/super8.cfg)

```
    # EXP1 header
    EXP1_1=PE12, EXP1_3=PB2, EXP1_5=PC14, EXP1_7=PG14, EXP1_9=<GND>,
    EXP1_2=PE13, EXP1_4=PG8, EXP1_6=PC13, EXP1_8=PG13, EXP1_10=<5V>,
    # EXP2 header
    EXP2_1=PA6, EXP2_3=PB7, EXP2_5=PB6, EXP2_7=PG15,  EXP2_9=<GND>,
    EXP2_2=PA5, EXP2_4=PA4, EXP2_6=PA7, EXP2_8=<RST>, EXP2_10=<5V>
```

### Fly Super 8 Pro

 - Main page for the [Fly Super 8 Pro](./fly-super8_pro_general.html)
- [Download a copy of the Super 8 Pro aliases file](./files/super8/super8.cfg)

```
    # EXP1 header
    EXP1_1=PE12, EXP1_3=PB2, EXP1_5=PC14, EXP1_7=PG14, EXP1_9=<GND>,
    EXP1_2=PE13, EXP1_4=PG8, EXP1_6=PC13, EXP1_8=PG13, EXP1_10=<5V>,
    # EXP2 header
    EXP2_1=PA6, EXP2_3=PB7, EXP2_5=PB6, EXP2_7=PG15,  EXP2_9=<GND>,
    EXP2_2=PA5, EXP2_4=PA4, EXP2_6=PA7, EXP2_8=<RST>, EXP2_10=<5V>
```

### Fly 407ZG

 - Main page for the [Fly 407ZG](./fly_407zg.html)
- [Download a copy of the Fly 407ZG aliases file](./files/fly-407zg/FFLY_407ZG.cfg)

```
    # EXP1 header
    EXP1_1=PB10,  EXP1_3=PE14,  EXP1_5=PE10,   EXP1_7=PE8,  EXP1_9=<GND>,
    EXP1_2=PE15,  EXP1_4=PE12,  EXP1_6=PE9,   EXP1_8=PE7,  EXP1_10=<5V>,
    # EXP2 header
    EXP2_1=PB14, EXP2_3=PC5,  EXP2_5=PC4,  EXP2_7=PB2,   EXP2_9=<GND>,
    EXP2_2=PB13, EXP2_4=PF11,  EXP2_6=PB15,  EXP2_8=<RST>, EXP2_10=<NC>,
```


### Fly Gemini V2

 - Main page for the [Fly Gemini V2](fly-gemini_v2_general.html)
- [Download a copy of the Fly Gemini V2 aliases file](./files/gemini_v2/FLY_GEMINI_V2.cfg)

```
    # EXP1 header
    EXP1_1=PC9,  EXP1_3=PA13,  EXP1_5=PA9,   EXP1_7=<NC>,  EXP1_9=<GND>,
    EXP1_2=PB6,  EXP1_4=PA10,  EXP1_6=PA8,   EXP1_8=<NC>,  EXP1_10=<5V>,
    # EXP2 header
    EXP2_1=PB14, EXP2_3=PA15,  EXP2_5=PA14,  EXP2_7=PC10,   EXP2_9=<GND>,
    EXP2_2=PB13, EXP2_4=PB12,  EXP2_6=PB15,  EXP2_8=<RST>, EXP2_10=<NC>,
```

### Fly Gemini V3

 - Main page for the [Fly Gemini V3](fly-gemini_v3_general.html)
- [Download a copy of the Fly Gemini V3 aliases file](./files/gemini_v3/FLY_GEMINI_V3.cfg)

```
    # EXP1 header
    EXP1_1=PC9,  EXP1_3=PA13,  EXP1_5=PA9,   EXP1_7=<NC>,  EXP1_9=<GND>,
    EXP1_2=PB10,  EXP1_4=PA10,  EXP1_6=PA8,   EXP1_8=<NC>,  EXP1_10=<5V>,
    # EXP2 header
    EXP2_1=PB14, EXP2_3=PA15,  EXP2_5=PA14,  EXP2_7=PA7,   EXP2_9=<GND>,
    EXP2_2=PB13, EXP2_4=PB12,  EXP2_6=PB15,  EXP2_8=<RST>, EXP2_10=<NC>,
```
