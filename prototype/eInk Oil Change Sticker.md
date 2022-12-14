![Affinity Designer](https://a11ybadges.com/badge?logo=affinitydesigner)![Node-RED](https://a11ybadges.com/badge?logo=nodered)![Home Assistant](https://a11ybadges.com/badge?logo=homeassistant)![Telegram](https://a11ybadges.com/badge?logo=telegram)

WORK IN PROGRESS

## Quick Setup

1) Setup Home Assistant Helpers
	- Odometer
	- Service Miles
	- Service Date
	- Binary Input - (Service Due Now)
2) Copy `fonts` folder to `/share/`
	- This is parent to the config folder usually shown to you in the file editor/ VS Code Server
3) Import Node Red Flow
	- Set Telegram info
4) Use app to transfer image to display
	- iOS:
	- Android:

## TL;DR

Use Home Assistant, Node Red, and an NFC powered ePaper display to track and display when vehicle maintenance should happen.

## Overview

Waveshare offers several ePaper displays for making prototypes, more recently they started offering some displays that are capable of being updated from a phone app via NFC. Power from the data transfer is harvested to refresh the screen, negating the need for a battery. Due to the nature of ePaper tech, the image is held infinitely. 

Their 2.1" and 2.9" seem to be a nice replacement for the sticker commonly given at oil change locations. This was built for the 2.9" display but can be easily adaptable.

## Logic

- Get Home Assistant to calculate `future date` and `future mileage` from current `odometer mileage`
	- Node Red generates image with data and sends to phone via Telegram


## Node Red

### Image base

I originally generated two images with the JIMP plugin and merged them, but the next modification complained about this so starting with a Base64 PNG is probably best, you can create one in your own design app and convert it here: https://codebeautify.org/base64-to-image-converter

Waveshare NFC Screens size reference:
- 2.9"  - 296x128 - `Used in this project`
- 2.7" - 264x176 - `Bare PCB`
- 2.12" - 250x122

### Fonts

Fonts for JIMP are bitmap FNT fonts and you'll need to convert any TTF/OTF fonts for every color and size you want to use: https://ttf2fnt.com/

## Questions

How to trigger? 
Needs odometer to be updated with trigger - or before - or after




## Research

The app used by the display wants an image to send to the display and programmatically generating an image with text is very new to me. Writing a Home Assistant custom integration is currently out of my grasp so I checked to see if I could do anything with Node Red.

![[/extras/media/FD306605-F93F-43FF-905E-71DA8D2EF164_1_105_c.jpeg]]![[/extras/media/Screenshot 2022-12-19 at 10.21.45 PM.png]]