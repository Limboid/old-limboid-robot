# Skeletal System

## Description

An assembly of articulating parts providing structural support. Actuated by muscular system.

## Composition

The many parts of the skeleton are categorized into either sub-assemblies or as 'inter-assembly' parts. Sub-assemblies defined many parts in a single CAD file while inter-assembly parts are solitary in their own file. Prefix 'L/R' indicates this part is only being defined for the left side, but X-axis mirror is needed to define the right part.

### Sub-assemblies

- head
- superior spine
- L/R shoulder
- L/R elbow
- L/R wrist
- L/R hand
	- base
	- thumb
	- pointer finger
	- middle finger
	- ring finger
	- pinky finger
- pelvic joint
- L/R hip joint
- L/R knee
- L/R ankle
- L/R foot

### Inter-assembly parts

- L/R humerus beam
- L/R radius and ulna beams
- spine beam
- pelic beam
- L/R femur beam
- L/R ftibia beam

## Production

0. Finalize parametrics
	- skip this if you are not changing any global parameters
	1. Enter appropriate values in 'global' spreadsheet [Data.FCStd]()
	2. For each FreeCAD file in [CAD]():
		0. while [Data.FCStd]() is already open, within the FreeCAD application open the file being updated
		1. execute python code:
			~~~
			for obj in App.ActiveDocument.Objects:
				obj.touch()
			App.ActiveDocument.recompute()
			~~~
1. For each subassembally or interassembally part, follow produce.txt
2. Assemble according to subassembally files and human anatomical resemblence

### Sources

After sourcing locally, stock components referenced in produce.txt files can be obtained from
| Items | Notes | URL | 
| ----- | ----- | --- |

## Interfaces

- ligaments connect muscles to bones and are defined in the muscular system. However in some very small parts, care is taken to ensure there is a suitable attachment site on the geometric surface of skeletal parts.
- most systems non-intrusively secure themselves on the skeleton
- fingertip cavities of fixed size host whatever sensors the signal system would like to squeeze in. while cavity dimensions are defined in the skeletal system, sensors embedded there are defined in the signal system.
- The head accommodates many electrical components. These are first defined in the signal or power systems. Then room is made in the skull to host these demands and best route a forced convection heat sink. Hosted components are:
	- charger
	- power button
	- eyes
	- ears
	- screen
	- speaker
	- computer
	- brain board
	- overheating temperature sensors
	- accelerometer
- The hydraulic system connects at the input and output ports for the skull's convection heat sink flow. The flexible tube delivering this flow is defined by the hydraulic system. Built in internal skull barbs and glue fix the tubes in place.
- The integumentary system stops at the base of the skull where its skull termination ring directly screws into the skull. Pitch, diameter and other details are defined in the skeletal system skull and conformed to by the integumentary system.
- Gloss and finish applied to skull (if any) is defined by the integumentary system.