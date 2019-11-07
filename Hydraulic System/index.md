# Hydraulic System

## Description

Provides controlled hydraulic power to muscles and circulates convection coolant

## Composition

In addition to ([hydraulic_system.FCStd][]), this system is described in various other places and can be decomposed as follows:
- Hydraulic core ([hydraulic_system.FCStd][]): supports all hydraulic system components
- Prime Mover:
	- (2) stator ([stator.FCStd][]): produces rotating magnetic field augmented by second-order magnetic coupling
		- electromagnet coils
		- temperature sensors
		- magnetic coupling bars: longtitudal external steel bars reducing magnetic field strength by interference
		- core: electromagnetic core, sensory host, and coolant tube
	- (2) rotors ([rotor.FCStd][]): convert rotating magnetic fields into mechanical rotation which pumps fluid in positive displacement fashion
		- house: externally positive displacement pump rotor, internally houses magnets
		- magnets: hallbach magnet array
	- shell: encompasses stators
- (N) Valves ([valve.FCStd][]): staged hydraulic valve starting with a motor to direct successively larger hydraulic fluid flows
- skull coolant flow lines: circulate coolant to skull

## Production

1. 3D Print
| Quantity | Part | design | material | print settings |
| -------- | ---- | ------ | -------- | -------------- |
| 2 | stator core | 'stator core' in [stator.FCStd][] | waterproof, iron powder infused filament | 100% infil |
| 2 | rotor house | 'rotor house' in [rotor.FCStd][] | waterproof | |
| 1 | hydraulic core | 'hydraulic core' in ([hydraulic_system.FCStd][]) | waterproof | |
2. Source
| Quantity | Part | specs | potential sources |
| -------- | ---- | ----- | ----------------- |
| 100 | TODO | no hay | no se |
3. Fabricate printed circuit board for [hydrologic_controller/hydrologic_controller.KiCAD]()
	- see 'PCB Production' under 'Production Technologies' in this project's README.md for help
4. list specific steps to assemble hydraulic core
5. end with how to mount to skeleton

## Interfaces

Being the glue between physical and virtual, the hydraulic system must be well defined to ensure no design overlap or competition with interfacing systems.
- hydraulic fluid lines transmiting hydraulic power to muscles are defined by the muscular system
- electromagnets and embedded sensors (in prime mover or valves) belong to hydraulic system, but since there is no reason to unnecessarily use wires, sufficient extra terminal wire is left to be directly used by the signal system
- flexible tube connecting to the input and output ports for the skull's convection heat sink flow are defined by the hydraulic system. However, internal skull barbs and glue belongs to the skeletal system