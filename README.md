# Limboid

Limboid robot design, production notes, and performance reviews

## Design Conventions

We describe the Limboid as the integration of 6 systems: power, hydraulic, locomotive, integumentary, signal, and control system. Although distinct, observe their connectedness in information transfer (Control > Signal > Hydraulic > Locomotive), end effector support (Integumentary, Locomotive, and Hydraulic work togethor), and enegry flow (Integumentary (charger) > Power > Hydraulic > Locomotive).

Every subsystem is listed in its own directory containing `index.md` which details the system's:
name
description
interfaces
production method

Additionally, some systems are composed of subsystems which follow this same description style.
