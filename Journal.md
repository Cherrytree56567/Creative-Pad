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

# August 7th: PCB rewiring

I redesigned the schematic with KiCad Parts and I used [KiCad Minimal](https://github.com/janelia-kicad/RP2040_minimal) as a starting point for the RP2040 schematic part. I also was able to reorganize and re-wire up the board. But it seems that I have done something wrong here. I don't think it is supposed to look like this. This could be because my wires were too close together. I also migrated my footprints, symbols and 3d models to the git repo, so you can recreate it too. PS: I fixed the USB C Port too.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/7..png?raw=true)

**Total time spent: 3h 9m 29s**

# August 8th: 3D Modelling

I finished the pcb so now I needed to make a case for it. I opened up OnShape and started making drawings of the pcb. Turns out, these drawings are really really high quality. Which means that it would have a ton of entities, which OnShape can't process. So I spent a ton of time cleaning up these parts in Affinity Designer. I still need to figure out the z heights for the case. I also added some M2 mounting holes for my pcb for it to connect together to the case. Anyway, here is a quick screenshot.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/8..png?raw=true)

**Total time spent: 2h 56m 08s**

# August 9th: Sketching

I had to do a ton of stuff like simplyfing the drawing for the bottom and the top. I also needed to measure how big the hotswap switch parts were so that I could indent them into the bottom case of the pcb. Simplyfing the drawings were very repetitive because I would need to remove and move a ton of parts and redo it a bunch of times (16 times). Ive finished the bottom casing, I still need to do the top and the glass bit for the display.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/9..png?raw=true)

**Total time spent: 1h 44m 31s**

# August 10th: Part Studio Sketches

I added MX Switches to Creative Pad PCB Assembly so that I could turn it into a simplified drawing. I used Fastened Mates to easily connect the MX Keys to the pcb. I may have misaligned it a bit, but it shouldn't be a huge issue. I was able to put my simplified drawing in OnShape's part studio. Then I added some padding to the switches because without it, even a slight misalignment would prevent it from going in the case.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/10..png?raw=true)

**Total time spent: 1h 37m 00s**

# August 11th: Indents and LCD Glass Layers

So I was able to finish my drawing and also create the Glass Bridge for my LCD. Unfortunately the glass bridge will have to be large. I was also able to create padded indents in my top case to accommodate the MX Switches. I still need to test everything in an assembly. I also created indents for the Knobs.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/11..png?raw=true)

**Total time spent: 1h 33m 00s**

# August 12 - 13th: Custom Key Caps

So I took a bit of inspiration from Teenage Enginerring and so I came up with these keycaps. It makes them look a lot of a music producer's synth board. Anyway, making this key cap took a ton of time because I needed to get the exact measurements and stuff for the MX Switch.

![](https://github.com/Cherrytree56567/Creative-Pad/raw/main/Demos/12..png?raw=true)

**Total time spent: 1h 22m 00s**