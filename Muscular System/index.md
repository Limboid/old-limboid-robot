# Muscular System

## Description

A collection of muscles actuating the skeletal system.

## Composition

A muscle is cotractable soft actuator composed of:
- ligaments: durable wire attatched to a question mark screw or directly sewn onto skeleton
- distal end cap: two parametrically defined plastic parts holding contractable region to ligaments
- proximal end cap: two parametrically defined plastic parts holding contractable region to ligaments and connecting hydraulic fluid line
- contractable region: watertight flexible tubing surrounded by a plastic braided sleeve that collectively can contract under higher pressure or rest at full length
- hydraulic fluid line: flexible tubing that delivers hydraulic fluid
- small amount of glue: seals muscle seams

![individual muscle assembly from muscular system](single_muscle_assembly.png)

Parametrics for all muscles in the muscular system muscles are listed in the 'All_Muscles' spreadsheet in [musclar_system.FCStd]().
| Parameter Name | Allowed Values | Description |
| -------------- | -------------- | ----------- |
| proximal attatchment | any attatchment site | where to make ligament anchor to limboid |
| proximal ligament | 'hook' or 'screw' | whether the wire is directly sewn into the site or connected by a question mark shaped screw |
| distal attatchment | any attatchment site | where to make ligament anchor to limboid |
| distal ligament | 'hook' or 'screw' | whether the wire is directly sewn into the site or connected by a question mark shaped screw |
| small | 0 or 1 | whether the muscle has small profile or not |
| large | 0 or 1 | whether the muscle has large profile or not |
| tube length | length | exposed length of relaxed constrictable muscle tubing |
| hydraulic line length | length | length of line delivering hydraulic fluid and energy to muscle from hydraulic core |

## Production

1 Purchase the required length/amount of items listed in the 'Purchase' spreadsheet in [musclar_system.FCStd]() by visiting the linked sources and entering the correct values. At times, notes are supplied to help.
2 3d print the required amount of 'large distal end cap', 'large proximal end cap', 'small distal end cap', and 'small proximal end cap' parts in [muscular_system.FCStd][], as directed by the '3D Print' spreadsheet in [musclar_system.FCStd][].
	- if you want to ensure fit, first print a few and test them with the tubing you ordered. Adjust parameters in 'Globals' spreadsheet in [musclar_system.FCStd][] as needed
3 Assemble muscles
4 Glue wires and tubing in place
5 Attatch to skeleton

## Interfaces

- hydraulic fluid lines: proximally connected with hydraulic system but defined as part of muscles
- ligaments: attatched to most bones without beforehand analysis. These are not defined in skeletal system. However, in some cases, precision demands the attatchment site specified on the bone design. In these cases, the interfacing attatchment site geometry is defined in the skeletal system but the ligament parts themselves are still defined under the muscle.
- contracted diameter: in some cases, negligable, but for larger muscles, may be factored in when specifying dimensions for integumentary system. Appropriate parameters defined in muscular system.