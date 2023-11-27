---
title: "Benchmarking different Microcontroller for maximum FPS with an SSD1306 OLED"
date: 2022-07-31T17:00:57+02:00
draft: true
summary: ""
tags: []
---

## TODO

- first
- second
- third

# I2C Frequency Results

| Device                       | µC Freq [MHz] | I2C Freq [kHz] | Freq (Oszi) | Library  | FPS | Notes                                                                                               |
| ---------------------------- | ------------- | -------------- | ----------- | -------- | --- | --------------------------------------------------------------------------------------------------- |
| KeeStudio Uno Plus           | 16            | 400            | ~ 400       | Adafruit | 23  |                                                                                                     |
| KeeStudio Uno Plus           | 16            | 800            | ~ 700       | Adafruit | 28  | Higher freq had no effect.                                                                          |
| KeeStdudio Mega 2560         | 16            | 800            |             | Adafruit | 28  | Same as Atmega328, same µC freq after all                                                           | 
| [[NodeMCU]] with [[ESP8266]] |               | 400            | ~ 400       | Adafruit | 36  | [[ESP8266]] don't have hardware I2C, so this is all in software. Amazing that it's still this fast. |
| [[NodeMCU]] with [[ESP32]]   |               | 800            | ~ 650 (wtf) | Adafruit | 64  |                                                                                                     |
| [[NodeMCU]] with [[ESP32]]   |               | 1000           | 70          | Adafruit | 76  | Even with higher freq, won't actually be faster. Still awesome though!                              |

## [[ESP8266]], [[NodeMCU]], [[ESP32]]

The GPIO numberings on these are a bit odd. They don't have hardware I2C, but the software implementation still has default, see [[NodeMCU#Pinout]]. 

| Pin | GPIO  | Use |
| --- | ----- | --- |
| D1  | GPIO5 | SCL |
| D2  | GPIO4 | SDA | 

For the [[ESP32]], the default Pins are:

| Pin | GPIO  | Use |
| --- | ----- | --- |
| G21  | GPI21 | SDA | 
| G22  | GPI22 | SCL |


# References