![image](https://github.com/xperiments/p1touch/assets/417709/0131a007-0720-47a0-a92a-47130f6b1577)

# Bambulab P1 Series Printer Screen

![image](https://github.com/xperiments/p1touch/assets/417709/cc6dd9ed-5c0f-4396-8859-09d312bc84a9)

This repository contains the design files and resources for the screen of the Bambulab P1 Series printer. The screen serves as the user interface for controlling and monitoring the printer's functions and settings.

# Required Hardware

Currently is has been only tested in the Cheap 2.8 inch ESP32-2432S028R board you can buy it here:

![image](https://github.com/xperiments/p1touch/assets/417709/28bdca76-9e49-4aab-a4c1-b714546077b4)
![image](https://github.com/xperiments/p1touch/assets/417709/658061e4-d638-4d1e-ab99-268baba40ebc)

[https://fr.aliexpress.com/item/1005004502250619.html](https://fr.aliexpress.com/item/1005004502250619.html)

In the future maybe I refactor it to the 5inch or 7inch

## Install drivers

[https://learn.sparkfun.com/tutorials/how-to-install-ch340-drivers/all](https://learn.sparkfun.com/tutorials/how-to-install-ch340-drivers/all)

## Some info about the board itsetlf

[https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/tree/main](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/tree/main)

## Features

The Bambulab P1 Series Printer Screen includes the following features:

Home

![image](https://github.com/xperiments/p1touch/assets/417709/d4362f14-6000-4e61-a8b1-98c78bc3fbaf)


- Displays the status of WiFi, Camera Recording, and Timelapse
- Provides a button for turning the light on/off
- Shows printer status when not printing
- When printing, it allows users to pause, resume, and stop the printing process
- Displays the remaining time and layers
- Allows users to adjust the printing speed

Temperatures

![image](https://github.com/xperiments/p1touch/assets/417709/5c66aa15-c7a5-43f0-94cd-6fd1042a5a21)
![image](https://github.com/xperiments/p1touch/assets/417709/e7b05b91-c94d-47a3-a35d-47c9d7832618)

- Allows users to set the target temperature for the bed and nozzle
- Provides options to control the fan speed for the part and auxiliary (to be enabled in settings, work in progress)

AXIS Control

![image](https://github.com/xperiments/p1touch/assets/417709/48c8f02b-35fe-489e-94aa-30c8ed870b00)

- Enables users to move the printer in the XY and Z directions
- Allows users to home the XYZ position
- Provides the option to change the movement steps from 1mm to 10mm

Filament (WIP)

![image](https://github.com/xperiments/p1touch/assets/417709/5229bed9-44c8-44d8-8c92-cf6aa5c9f429)

- Offers functionality for purging and retracting filament
- Allows users to load and unload filament (work in progress)

Settings

![image](https://github.com/xperiments/p1touch/assets/417709/5b6581ee-967c-4d93-83bf-d789af94c83a)
![image](https://github.com/xperiments/p1touch/assets/417709/f75ac87b-5568-4497-88d4-27c9585fbdc9)

- Enables users to activate the auxiliary fan if installed
- Allows users to enable the chamber sensor (to be determined, work in progress)
- Provides options to reboot the device
- Allows users to reset the touch configuration, which will be applied upon reboot
- Offers the ability to restore default settings for WiFi and P1PTouch configurations

# Installation

Use the [Online Web Installer](https://xperiments.in/p1touch/webusb)

# Setup

## With your phone, connect to the P1PTouch Network. Password is 12345678
<img src="https://github.com/xperiments/p1touch/assets/417709/a3c6f096-bb0b-4e8c-a006-34d0446d12d5" width="320"/>

## Configure Your Router WiFi nextwork & password
<img src="https://github.com/xperiments/p1touch/assets/417709/668c073c-c80f-44ab-962c-788e57ddf42d" width="320"/>

## Configure Your P1P/P1S settings
<img src="https://github.com/xperiments/p1touch/assets/417709/1136271d-d3c8-4ef2-ad56-a62f9d4f568a" width="320"/>

## Save settings and continue connection in the P1Touch Screen.
### First time you need to calibrate touch sensor. Just tap with the stylus in the cross.

<img src="https://github.com/xperiments/p1touch/assets/417709/69f77a07-08a0-4df8-a26a-f31cb12d6ec9" width="320"/>



