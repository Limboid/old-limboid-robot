# Limboid

Limboid design, operation, and production repository. For project details, see [limboid.ai].

## Design Conventions

We describe the Limboid as the integration of 6 systems: power, hydraulic, locomotive, integumentary, signal, and control system. Although distinct, observe their connectedness in information transfer (Control > Signal > Hydraulic > Locomotive), end effector support (Integumentary, Locomotive, and Hydraulic work togethor), and enegry flow (Integumentary (charger) > Power > Hydraulic > Locomotive). As the Limboid evolves, no doubt more systems will join these 6 as these become increasingly integrated. 

Every subsystem is listed in its own directory containing `index.md` which details the system's:
- description: what it is and a overview of composition. If composed of subsystems, assemballies, or components, these appear here
- interfaces: components of this system that are shared with other systems
- production method: precise details including links to files to produce the system

As each system deals with its own domain of science, engineering, and technology, a subsection labeled `Terminology` appears at times disambiguating the description language that follows.