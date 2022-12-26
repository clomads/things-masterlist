
[![obsidian](https://img.shields.io/badge/Made%20with-Obsidian-blue?style=flat-square&logo=obsidian)](https://www.obsidian.md)
[![ko-fi](https://img.shields.io/badge/Buy%20Me%20A-Coffee-red?logo=ko-fi&style=flat-square)](https://www.ko-fi.com/clomads)
[![Support me on Patreon](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dclomads%26type%3Dpatrons&style=flat-square)](https://patreon.com/clomads)
![GitHub](https://img.shields.io/github/license/clomads/Mato-Mini-M1?style=flat-square&logo=creative%20commons)

# @clomads "Things Masterlist"

## TL;DR

I make things: 3D models, PCBs, other prototypes. This is very incomplete documentation of those things that don't yet have or won't have their own repo.

It's probably mostly focused on 3D models I make in Fusion 360, but there's gonna end up being a lot here.

***Please support my work via Patreon, Ko-Fi, Venmo, Paypal, Cash App, etc. so I can continue making things.***

***I also sell some things at [vdbx.io](http://vdbx.io)***

## Overview

I (Chloe Madison / @clomads) originally bougt a Monoprice Maker Select v2.1 in 2017 and began to learn Fusion 360 via the maker license. I quickly decided to open source everything I made while selling production pieces through my brand Voidbox Industries (vdbx.io)

Problem is that documentation is hard and doesn't feed the ADHD need for dopamine like the design process does. It is now 2022 going into 2023 and I am just now getting around to properly exporting and sharing everything.

Most things are random and will be housed in this repo as a master list companion to individual listings on Printables, Thingiverse, etc. Some projects may get their own repo depending on a multitude of factors and I'll do my best to link them here.

### Current Hardware
**Creality Ender 3 v2 (32 bit + Silent stepper drivers)**
- Klipper on Raspberry Pi 3 via Mainsail OS
	- Custom enclosure w/ 30A DC relay
		- Mainsail connection to Home Assistant (not great ATM)
	- DC powered from 24v lithium solar battery (I live in a bus)
		- DC to DC buck conversion to maintain voltage
		- House batt is usually above 25v and charges to 29.4v (7s NMC)
- Upgraded Metal Hobbed Extruder Gear
- Satsana Hot End Cooler with BL Touch

### Future Hardware

**Support My Work**
Help me upgrade my system if you like what you see. I have a Patreon for monthly contributions and a Ko-Fi/Venmo/Cash App/Paypal for one-time tips. You can also find stuff of mine to buy all over the internet - I'm trying my best to get it all together. 

- Revo Hemera XS w/ full nozzle set 
- obXisian Revo nozzles


### VDBX.io

Voidbox Industries is the brand I sell my marketable designs under and most of those designs have their own repos and have obtained OSHWA certification, stating that they are truly open source. Voidbox has its own Github profile where you can find everything including the custom circuit boards I've been focused on since COVID.  

The current list of VDBX 3D models is:

- [Concrete Business Card Holder](https://github.com/vdbxio/clomads-card-holder) - `OSHWA US000129`
- [Hactus](https://github.com/vdbxio/Hactus) - `OSHWA US000196`
- Concrete Soap Dish - `yet to be released`
- Handy Jr. - `yet to be released`
- Handy Sr. - `yet to be released`

## The Master List

Each folder in this repo represents a design/project and will have a `.F3D` export from Fusion 360 alongside `STL` / `3MF` files ready to be sliced.

I haven gotten better at building parametric when it makes sense or at least building in an order that prevents breaks with changes, but older designs and many new designs are hella messy. Feel free to contact me if you'd like help making modifications to a specific design.


## Notes about this repo

This repo is built as an Obsidian vault and contains extra files to support it as such. You should be able to clone it and open it with your own obsidian install. It is unlikely that anyone would contribute to this repo, but if you want to use it as a template for yourself the following files may be useful.

- `obsidian_template` - folder contains structural components to help write `README.md` files
- `TOOLS.md` - contains links to helpful tools that support the creation of this repo


## License

CC 4.0 BY-SA on most designs and documentation unless otherwise noted

remix freely - credit me - share with same license