# Limboid

Limboid design repository. Design problems can be raised in the issues section of this repo. See wiki for development and operations manual. For project overview, please visit [limboid.ai].

[picture of a limboid]

## Design Conventions

We describe the limboid as the composition of 7 systems: power, hydraulic, skeletal, muscular, integumentary, signal, and control system. Being such an integrated system of systems, these reduced systems do not form the purest model of the limboid. It may also be viewed from the perspective of differing signal mediums (AGI > computer > electrical signals > hydrologic signals > hydraulic flow > muscle actuation > skeleton locomotion), enegry transmission (battery > prime mover > muscles > skeleton), or anatomical location (head, left upper arm, etc., employing same descriptions used for humans) to name a few additional perspectives. Additionally, as the limboid evolves, no doubt more systems will join these 7 as they become increasingly integrated. 

Every subsystem is listed in its own directory containing `index.md` which details the system's:
- description: what it is
- composition: how the system is composed; its subassemballies and components
- production: steps to take after finalizing design and parameters to produce finished system
- interfaces: components shared across systems are noted here