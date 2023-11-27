---
title: "Monitor and Window Manager Latency Measurements"
date: 2022-07-31T17:03:52+02:00
draft: true
summary: ""
tags: []
---

## TODO

- Inspiration (HN)
- The Lag Meter
- Hard-and Software used (monitors, frequency, Window Manager)
- Results

# Results

Sorted from lowest latency to highest.

| System / OS                       | CPU      | Composer              | Program     | Monitor    | Refresh           | Mean | Std |
| --------------------------------- | -------- | --------------------- | ----------- | ---------- | ----------------- | ------------ | --- |
| Linux Console                     | R5 1600x | -                     | -           | Acer Right | 60                | 24           | 3   |
| Linux Console                     | R5 1600x | -                     | -           | Acer Left  | 60                | 25           | 3   |
| Linux Console                     | R9 3900X | -                     | -           | ASUS Main  | 60                | 30           | 4   |
| Grub                              | R5 1600x | -                     | -           | ASUS Main  | 60                | 33           | 5   |
| Linux KDE X370                    | R5 1600x | KWin Off              | Konsole     | ASUS Main  | 144               | 37           | 4   |
| Linux KDE X370                    | R5 1600x | KWin On               | Konsole     | ASUS Main  | 144               | 41           | 4   |
| Linux KDE X370                    | R5 1600x | KWin On               | Kitty       | ASUS Main  | 144               | 42           | 6   |
| Linux KDE X370                    | R9 3900X | KWin On               | Termux      | ASUS Main  | 144               | 43           | 2   |
| Linux KDE X370                    | R5 1600x | KWin On               | Kitty       | Acer Left  | 75                | 51           | 4   |
| Linux KDE X370                    | R5 1600x | KWin On               | Konsole     | Acer Left  | 75                | 55           | 2   |
| Linux KDE X370                    | R5 1600x | KWin On               | Kitty       | Acer Right | 75                | 55           | 11  |
| Linux KDE X370                    | R5 1600x | KWin On               | Konsole     | Acer Right | 75                | 58           | 6   |
| Windows 10                        | R5 1600x | Effects Off           | CMD.EXE     | ASUS Main  | 144               | 60           | 10  |
| Linux KDE X370                    | R9 3900X | KWin On               | VSCode      | ASUS Main  | 144               | 60           | 6   |
| Windows 10                        | R5 1600x | Effects On            | CMD.EXE     | ASUS Main  | 144               | 61           | 6   |
| Android, Pixel 3a                 | -        | -                     | Google Keep | -          | 60 (?)            | 62           | 8   |
| Android, Pixel 3a                 | -        | -                     | Termux      | -          | 60 (?)            | 65           | 9   |
| Linux KDE X370                    | R5 1600x | KWin On               | Konsole     | Acer Left  | 60                | 67           | 9   |
| VirtualBox, Linux Virtual Console | R9 3900X | KWin On (Host)        | -           | ASUS Main  | 144 real, 60 virt | 68           | 8   |
| Linux KDE X370                    | R5 1600x | KWin On               | Konsole     | ASUS Main  | 60                | 69           | 7   |
| VirtualBox, Linux KDE             | R9 3900X | KWin On (Host, Guest) | Konsole     | ASUS Main  | 144 real, 60 virt | 82           | 7   |
| Linux KDE X370                    | R5 1600x | KWin On               | VSCode      | ASUS Main  | 144               | 86           | 13  |
| VirtualBox, Linux KDE X370        | R5 1600x | KWin On (Host, Guest) | Konsole     | ASUS Main  | 144 real, 60 virt | 107          | 16  |


# References