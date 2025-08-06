---
Title: "Creative Pad"
Author: "CT5"
Description: "A simple Macropad with an OLED with knobs with a futuristic design with a custom microcontroller pcb."
Created On: "31/07/2025"
---

# July 31st: Created the Keys and the Microcontroller stuff!

I created a simple project in Easy EDA and I was able to create a bunch of mini parts for the microcontroller.
I was able to get a voltage converter which converted it from 5V to 3V3 for the RP2040. I also got some key switches and stuff in order. I plan to add a knob and a screen (KWH030ST11-F02) later on. Here is a picture of my schematic.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/1..png?raw=true)

**Total time spent: 1h 31m 51s**

# August 1st: Added the Potentiometer and recreated stuff!

Turns out, you need to save in EasyEDA. I though it autosaved because it was an online program. Anyway, so I had to recreate most of the rp2040 stuff.
I also added a potentiometer and finished the rp2040 stuff. Im using the rp2040 [example](https://easyeda.com/editor#id=!757ac41db9974acda8ffcb7bf90f7860) on Easy EDA.
I didn't fully copy it (because you can't copy from std to pro) and I modified it a bit and did a bit of parts searching. I also organised it a bit.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/2..png?raw=true)

**Total time spent: 2h 14m 12s**

# August 2st: Added a display!

Finding a display that was compatible is really really hard. Because you need to find one that exactly matches the size. I was able to find a display that matched. I also needed to convert the 3V3 Voltage to 2V8.
So I was able to use an LDO Regulator to regulate the voltage to 2V8 and connect it to the RP2040. I was considering changing the microcontroller to the RP2350B, but considering that the RP2350B had way too many pins it would have been way harder. For the display I've used an FPC connector to connect the display. I still need to figure out how I am going to connect the display to the glass front.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/3..png?raw=true)

**Total time spent: 2h 7m 50s**

# August 3rd - 4th: Migrated to Kicad

I tried using EasyEDA's pcb creation tool online on Edge, because it was unsupported on firefox, but after 30mins I saw that it was much more difficult than I thought because some features on EasyEDA were missing that were avaliable on KiCAD. After a long time, I was able to migrate everything to Kicad, and almost finish doing the switch bits. Since I'm already used to Kicad, it was much easier. I was able to use the program EasyEDA2Kicad on Python to convert EasyEDA models to Kicad so that I could effectivly migrate it.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/4..png?raw=true)

**Total time spent: 6h 16m 40s**

# August 5th: Kicad-Wakatime and Hotswap

I've migrated to KiCad-Wakatime, but before that I was using a stopwatch. My stopwatch said 21 mins before I started groundplane so Im adding it to the total time. Also I tried using Scotto Keebs' Hotswap footprint on Kicad, but it is difficult to use. So I found this opensource one on github that was avaliable on the KiCad Plugin Manager. I swapped all my switches to MX HotSwap. I was also able to organize all the components and put all of the diodes, resistors, capacitors, screen, microcontroller, regulators and diodes in their respective places.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/5..png?raw=true)

**Total time spent: 1h 12m 37s**

# August 6th: Schemetic Redesign

I had to redesign the schematic because the parts and footprints which I used in Easy EDA were difficult to use in KiCad. Im going to finish doing the rest tomorrow. I also need to rewire the pcb. This is especially difficult because of the limited space avaliable in the board. Unfortunatly, I only realised that EasyEDA footprints wouldn't work in KiCAD after I finished wiring it up. So here is quick screenshot.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/6..png?raw=true)

**Total time spent: 1h 22m 25s**