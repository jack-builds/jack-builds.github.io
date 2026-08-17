# ☕ Coffee Lab

Coffee Lab is my long-term project to build a **custom, open-source, ridiculously over-engineered coffee machine**.

The idea started with wanting to build my own coffee maker, but it has evolved into a combination of coffee, electronics, programming, 3D printing, CAD, PCB design, and automation.

## The Vision

I want Coffee Lab to eventually be a beautiful ~2-foot-tall machine with:

- A clear enclosure so you can see everything happening
- Wood and aluminum construction
- Clear tubing and some copper components
- A custom brew chamber
- Precise temperature control
- Precise water delivery
- A load-cell-based scale
- Custom PCBs
- Modular electronics
- A touchscreen
- A Raspberry Pi + ESP32
- A local web interface
- Eventually a mobile app
- A camera for monitoring
- Automated cleaning
- Local/offline AI
- And probably a ridiculous number of other features

The goal is to make **really good pour-over coffee**, while making the machine itself just as fun as the coffee.

## Electronics

The current computer architecture is:

**ESP32-S3** → controls the actual machine

**Raspberry Pi 4** → touchscreen, website, monitoring, camera, and eventually AI

They will communicate over UART.

I'm also designing the electronics around a **modular PCB system**. Instead of putting everything on one giant PCB, the machine will have a mainboard/backplane with replaceable modules such as:

- Power
- Motion
- Sensors
- AUX
- Expansion

That means I can replace or upgrade individual modules without replacing the entire machine.

Eventually, I want to design my own PCBs in **KiCad** and have them manufactured by **JLCPCB**.

## Current Hardware

Some of the parts I'm starting with include:

- Adafruit ESP32-S3 Feather
- Raspberry Pi 4 8GB
- NEMA 17 stepper motor
- TMC2209 stepper driver
- 3D-printed peristaltic pump
- PT1000 RTD
- MAX31865 temperature amplifier
- Mavin NA151 load cell
- HX711 load-cell amplifier
- 608 bearings
- Various electronics and prototyping parts

I'm also experimenting with a **SIMAX 1L GL45 laboratory bottle** as the water reservoir.

## The First Version

The first version doesn't need to be beautiful.

I want to get the basic system working first:

**Reservoir → Pump → Temperature control → Brew chamber → Coffee**

with the ESP32 controlling the hardware and the sensors providing feedback.

The first major milestone is simple:

> **Make a real cup of coffee with a machine I built myself.**

Then I'll keep improving it.

## Long-Term Goal

Eventually, I want Coffee Lab to become a fully open-source project where other people can build their own machines, modify them, design new modules, and contribute improvements.

Maybe someday there could even be DIY kits or official hardware modules.

But for now, I'm just trying to build the coolest coffee machine I possibly can.

**☕ Build it. Brew it. Upgrade it forever.**
