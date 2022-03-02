# Limboid

ℹ️ **This project has moved to [Limboid/limboid-robot](https://github.com/Limboid/limboid-robot).** 

Limboid design repository. Design problems can be raised in the issues section of this repo. See wiki for development and operations manual. For project overview, please visit [limboid.ai].

[picture of a limboid]

We describe the limboid as an integrated system of 7 systems: [power](power system/index.md), [hydraulic](hydraulic system/index.md), [skeletal](skeletal system/index.md), [muscular](muscular system/index.md), [integumentary](integumentary system/index.md), [signal](signal system/index.md), and [control](control system/index.md) system. Being such an integrated system of systems, these reduced systems do not form the purest model of the limboid. It may also be viewed from the perspective of differing signal mediums (AGI &rarr; computer &rarr; electrical signals &rarr; hydrologic signals &rarr; hydraulic flow &rarr; muscle actuation &rarr; skeleton locomotion), enegry transmission (battery &rarr; prime mover &rarr; muscles &rarr; skeleton), or anatomical situation (head, left upper arm, etc., employing same descriptions used in human anatomy) to name a few additional perspectives. Additionally, as the limboid evolves, no doubt more systems will join these 7.

## Quick Build

To quickly build your own limboid machine, visit our [Quick Build](https://www.youtube.com/playlist?list=PLJVJzDoCz7-sVb5Z7Gw86evb6sRxNrpWM) playlist. 

## Design Conventions

Every subsystem is listed in its own directory containing `index.md` which details the system's:
- description: what it is
- composition: how the system is composed; its subassemballies and components
- production: steps to take after finalizing design and parameters to produce finished system
- interfaces: components shared across systems are noted here

### Parametrics

Global variables referenced by GLOBAL_VAR_NAME appear at times within designs. Currently these variables are:

| Name | Domain | Notes |
| ---- | ------ | ----- |
| HEIGHT | 1 600 mm - 1 900 mm | |

### Coordinate System

Unless noted, files assume the XYZ axes to indicate right, forward, and upward respectively. In the case of symetric components, unless otherwise stated, merely reflecting along the X-axis gives an acceptable mirror.

## Production Technologies

### Simple Subtractive Operations

Many extruded parts need to be cut to length, drilled, or tapped for threads.

### PCB Production

Some of the PCB's for this project require very fine (0.15mm) traces. With propper technique however, this can be achieved with inkjet print, iron, disolve technology. The steps involved are:
1. TODO
2. LIST
3. STEPS

While you can buy time at an expert pcb fab shop, be warned, they often charge a lot for placing components. For this reason, we made a custom toolhead and control system that leeches onto a 3D printer to use machine vision to accurately apply solder paste and pick up and place components. The resulting board is then heated with the build platform at XXX&deg;C for 25min.

### Electronics Testing

A good multimeter should do the trick

### Thermoplastic Welding

Some operations require joining thin thermoplastic films to other thermoplastics. A handheld heat gun should produce acceptable results

### Aluminum Welding

Welding does in 1 operation what may require 10 elsewhere. With the lower density of aluminum, you may even get away with a high temperature solder gun. 

### 3D Printing

This project leans on 3D printing to produce numerous plastic parts, some waterproof and others with iron powder infused.

### Soft Finishing

The skull needs to be polished and coated in laquer and other 3D printed parts must be post processed to ensure precise fits.

### Coil Winding

A mounted drill makes quick work winding 60m of electromagnet coils.

### Assembly

Ultimately, components must be picked, placed, screwed, and otherwise assembled into the complete limboid machine.

## File Formats

Much of the Limboid is designed in [FreeCAD](https://www.freecadweb.org/), [KiCAD](http://www.kicad-pcb.org/), and [Modelio](https://www.modelio.org/). We strongly encourage contributers to continue using freely available engineering software.

### 3D Printing and FreeCAD

Since a 3D printing workbench is available for FreeCAD allowing users to directly 3D print parts in FreeCAD, there are no separate .stl files. These would take up space and get dated by changes in parametrics causing confusion.

## Issues

Please take advantage of Github's issue tracker, and we or the community can help. If it is very urgent, please email us at [help@limboid.ai](mailto:help@limboid.ai)
