---
title: "Pollin 7 Segment Displays"
date: 2022-07-31T17:05:43+02:00
draft: true
summary: ""
tags: [Electronics, SevenSegmentDisplay]
---

## TODO

- first
- second
- third

# 7 Segment Displays

I have several different 7 segment displays from Pollin. Some have a part number printed on them, most don't. These are my notes for them.

![[7_Segment_Display_with_Labeled_Segments.svg|200]]

# Single Segments

| Front | Back | LED Color | Case Color | Inscription | Pins | Common | Pinout |
| ----- | ---- | --------- | ---------- | ----------- | ---- | ------ | ------ |
|       |      |           |            |             |      |        |        |
	

# Dual Segments

Note: the first four seem to be from a similar series called 3021, 3022 or 3023. Sometomes 3201. They are 0.3in in length, on chinese seller pages sometimes 15.4x15x4mm. The dimensions are spot on.

![[Pasted image 20211015195457.png]]

| Front                                | Back                                 | LED Color | Case Color | Inscription                | Pins | Common  | Pinout           | Datasheet                           |
| ------------------------------------ | ------------------------------------ | --------- | ---------- | -------------------------- | ---- | ------- | ---------------- | ----------------------------------- |
| ![[PXL_20211012_081506685.jpg\|100]] | ![[PXL_20211012_081513274.jpg\|100]] | Red       | Grey       | Internal: A/B B3021 or 230 | 10   | Cathode | [[#Layout One]]  | [[D121543D.pdf]]                    |
| ![[PXL_20211012_081615479.jpg\|100]] | ![[PXL_20211012_081621835.jpg\|100]] | Red       | Black      | RX3201BR (LEDTECH LD3052)  | 10   | Anode   | [[#Layout One]]  | [[D121543D.pdf]], [[datasheet.pdf]] | 
| ![[PXL_20211012_081530619.jpg\|100]] | ![[PXL_20211012_081537250.jpg\|100]] | Red       | Green      | Internal: Cile 3023 E/F    | 10   | Anode   | [[#Layout One]]  | [[D121543D.pdf]]                    |
| ![[PXL_20211012_081603681.jpg\|100]] | ![[PXL_20211012_081608349.jpg\|100]] | Red       | Red        | Internal: 35C HP           | 10   | Cathode | [[#Layout One]]  | [[D121543D.pdf]]                    |
| ![[PXL_20211012_130921083.jpg\|100]] | ![[PXL_20211012_130927718.jpg\|100]] | Red       | Black      | LEDTECH 9.03 LA5052-11 H   | 18   | Anode   | [[#Layout Five]] | [[LA5052-11(1).pdf]]                |
	
# Triple Segments

| Front                                | Back                                 | LED Color | Case Color | Inscription           | Pins | Common  | Pinout          | Datasheet                |
| ------------------------------------ | ------------------------------------ | --------- | ---------- | --------------------- | ---- | ------- | --------------- | ------------------------ |
| ![[PXL_20211012_111338697.jpg\|100]] | ![[PXL_20211012_111344322.jpg\|100]] |           | Grey       | Kingbright BC56-11EWA | 28   | Cathode | See Datasheet   | [[BC56-11EWA-53157.pdf]] |
| ![[PXL_20211012_143349499.jpg\|100]] | ![[PXL_20211012_143352796.jpg\|100]] | Red       | Black      | Internal: P-3156      | 12   | Anode   | [[#Layout Six]] |                          |
	

# Quad Segments

| Front                                | Back                                 | LED Color | Case Color | Inscription           | Pins           | Common  | Pinout            | Datasheet             |
| ------------------------------------ | ------------------------------------ | --------- | ---------- | --------------------- | -------------- | ------- | ----------------- | --------------------- |
| ![[PXL_20211012_111302997.jpg\|100]] | ![[PXL_20211012_111313197.jpg\|100]] | Red       | Grey       | Sharlight CM4-028530L | 16 (1 missing) | Cathode | [[#Layout Two]]   |                       |
| ![[PXL_20211012_111416620.jpg\|100]] | ![[PXL_20211012_111421571.jpg\|100]] | Green     | Grey       | Sharlight CM4-040520L | 16 (2 missing) | Cathode | [[#Layout Three]] | [[D121534D(1).pdf]]   |
| ![[PXL_20211012_111320608.jpg\|100]] | ![[PXL_20211012_111326583.jpg\|100]] | Red       | Red        | Internal: SL-304C     | 24             | Cathode | [[#Layout Four]]  |                       |
| ![[PXL_20211012_143337478.jpg\|100]] | ![[PXL_20211012_143342873.jpg\|100]] | Green     | Grey       | Kingbright CC56-21GWA | 12             | Cathode | [[#Layout Six]]   | [[CC56-21GWA(1).pdf]] |


# Layouts

## Layout One

As seen from top, so LEDs are visible. Numbering goes bottom left -> bottom right -> top right -> top	 left.

| Pin | Connection         | Position     |
| --- | ------------------ | ------------ |
| 1   | G                  | Bottom Left  |
| 2   | DP                 |              |
| 3   | A                  |              |
| 4   | F                  |              |
| 5   | Common C/A Digit 2 | Bottom Right |
| 6   | D                  | Top Right    |
| 7   | E                  |              |
| 8   | C                  |              |
| 9   | B                  |              |
| 10  | Common C/A Digit 1 | Top Left     |

## Layout Two	

As seen from top, LEDs are visible. Start bottom left -> bottom right -> top right -> top left

| Pin | Connection          | Position     |
| --- | ------------------- | ------------ |
| 1   | Common C/A Digit 1  | Bottom Left  |
| 2   | C  (L3)             |              |
| 3   | DP                  |              |
| 4   | NC                  |              |
| 5   | E                   |              |
| 6   | D                   |              |
| 7   | G                   |              |
| 8   | Common C/A Digit 4  | Bottom Right |
| 9   | NC                  | Top Right    |
| 10  | NC No Pin           |              |
| 11  | Common C/A Digit 3  |              |
| 12  | Common C/A L (Dots) |              |
| 13  | A (L1)              |              |
| 14  | Common C/A Digit 2  |              |
| 15  | B (L2)              |              |
| 16  | F                   | Top Left     |

## Layout Three	

As seen from top, LEDs are visible. Start bottom left -> bottom right -> top right -> top left

| Pin | Connection          | Position     |
| --- | ------------------- | ------------ |
| 1   | Common C/A Digit 1  | Bottom Left  |
| 2   | Common C/A Digit 2  |              |
| 3   | D                   |              |
| 4   | Common C/A L (Dots) |              |
| 5   | E                   |              |
| 6   | Common C/A Digit 3  |              |
| 7   | DP                  |              |
| 8   | Common C/A Digit 4  | Bottom Right |
| 9   | NC                  | Top Right    |
| 10  | NC No Pin           |              |
| 11  | F                   |              |
| 12  | NC No Pin           |              |
| 13  | C  (L3)             |              |
| 14  | A (L1)              |              |
| 15  | G                   |              |
| 16  | B (L2)              | Top left     |

## Layout Four	

| Pin | Connection             | Position     |
| --- | ---------------------- | ------------ |
| 1   |                        |              |
| 2   | Common C/A Digit 1     | Bottom Left  |
| 3   | D                      |              |
| 4   |                        |              |
| 5   | Common C/A Digit 2     |              |
| 6   | Cathode Middle Dots    |              |
| 7   | Anode Middle Dots      |              |
| 8   | Common C/A Digit 3     |              |
| 9   | DP3                    |              |
| 10  | Common C/A Digit 4     |              |
| 11  | E (Only Digits 2-4)    |              |
| 12  |                        | Bottom Right | 
| 13  |                        | Top Right    |
| 14  |                        |              |
| 15  |                        |              |
| 16  | Cathode DP3            |              |
| 17  | A                      |              |
| 18  | F                      |              |
| 19  | B                      |              |
| 20  | C                      |              |
| 21  | E (but only digit 1?!) |              |
| 22  | G                      |              |
| 23  |                        |              |
| 24  |                        | Top Left     |

## Layout Five

| Pin | Connection    | Position     |
| --- | ------------- | ------------ |
| 1   | F1            | Bottom Left  |
| 2   | D1            |              |
| 3   | C1            |              |
| 4   | DP1           |              |
| 5   | E2            |              |
| 6   | D2            |              |
| 7   | G2            |              |
| 8   | C2            |              |
| 9   | DP2           | Bottom Right |
| 10  | B2            | Top Right    |
| 11  | A2            |              |
| 12  | F2            |              |
| 13  | Anode Digit 2 |              |
| 14  | Anode Digit 1 |              |
| 15  | B1            |              |
| 16  | A1            |              |
| 17  | G1            |              |
| 18  | F1            | Top Left     | 

## Layout Six

Cannot Display Decimal Dots DP1-DP4 on 4 Digit Display.
Cannot Display DP3 on 3 Digit Display, Pin 6 is NC on 3 Digit.

| Pin | Connection                              | Position     |
| --- | --------------------------------------- | ------------ |
| 1   | E                                       | Bottom Left  |
| 2   | D                                       |              |
| 3   | DP5, DP6 (attached to Digit 3, Digit 4) |              |
| 4   | C                                       |              |
| 5   | G                                       |              |
| 6   | Common C/A Digit 4                      | Bottom Right |
| 7   | B                                       | Top Right    |
| 8   | Common C/A Digit 3                      |              |
| 9   | Common C/A Digit 2                      |              |
| 10  | F                                       |              |
| 11  | A                                       |              |
| 12  | Common C/A Digit 1                      | Top Left     |

# Drivers

## CD4511

Common Cathode, BCD Decoder

## CD4543

CMOS, both Common Anode and Cathode, BCD Decoder

## MAX7219

Uses SPI. Usually Common Cathode, but can do Common Anode as well with a trick:

![[4-Digit-CA.png]]

This is because the thing can drive 64 LED matrices as well, and they tend to have both. We loose 7 Seg decoder function this way, so we have to target the segments in software.

Datasheet: [[MAX7219-MAX7221(1).pdf]]

## TM1637

Uses a I2C-like protocol. Can do common anode and common cathode. Well supported by Arduino. 

# References

# References