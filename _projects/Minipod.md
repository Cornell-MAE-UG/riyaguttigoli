---
layout: project
title: "Cornell Hyperloop: MiniPod - Scaled Electromagnetic Levitation Platform"
description: Led the research, mechanical development, and magnetic levitation testing of a scaled Hyperloop platform integrating electromagnets, force characterization, precision air-gap sensing, and closed-loop levitation controls.
technologies: [MATLAB, Electromagnetic Design, Magnetic Circuit Modeling, Test Fixture Design, Load Cell Testing, PID Control, Sensor Integration, Automated Coil Winding, Rapid Prototyping, CAD, Systems Integration]
categories: [robotics, hardware, modeling, research]
card_tags: [Robotics, Hardware, Controls]
order: 1
image: /assets/images/minipod/coverpic.png
---

## Project Overview

<img src="{{ '/assets/images/minipod/coverpic.png' | relative_url }}"
class="overview-image">

The **MiniPod** is a scaled electromagnetic levitation platform developed by Cornell Hyperloop to mature magnetic subsystem technology before attempting integration on the team's full-scale pod. I was a founding member of the project as a sophomore on the Magnetics subteam and maintained ownership as I progressed into the roles of **Magnetics Lead** and later **Mechanical Team Lead**.

The project began as a low-cost proof of concept for demonstrating controlled magnetic levitation. Its purpose was not simply to construct a smaller pod, but to create an accessible test platform through which the team could characterize electromagnets, develop levitation controls, validate subsystem interfaces, and preserve technical knowledge for future Hyperloop vehicles.

Funding and manufacturing resources were major constraints throughout development. Rather than beginning with costly high-purity iron cores and fully customized magnets, we adopted an iterative strategy: first characterize modified off-the-shelf transformers, use those modules to develop the levitation controls system, and then transition toward custom-wound electromagnets as additional resources became available.

---

## System Architecture

The MiniPod combines electromagnetic levitation, mechanical guidance, a modular aluminum-extrusion chassis, air-gap sensing, power electronics, and closed-loop controls. My work focused on the mechanical architecture, levitation hardware, test fixtures, and interfaces between the magnetics, controls, power, and structural systems.

<figure class="project-figure">
<img src="{{ '/assets/images/minipod/system-architecture.png' | relative_url }}">
</figure>

---

## Phase 1: Low-Cost Levitation Modules

Because purpose-built electromagnets and high-purity iron cores were initially outside the team’s budget, we began with modified microwave transformers. The laminated cores were cut to expose a pre-wound coil and create an inexpensive proof-of-concept levitation module.

We characterized the modified transformers through B-H curve testing to estimate permeability, identify saturation, and establish safe operating limits. Testing indicated saturation near **8 A** and confirmed that the transformer cores were useful for early controls development but not ideal for long-term scalability.

<figure class="project-figure">
<img src="{{ '/assets/images/minipod/transformer-development.png' | relative_url }}">
<figcaption>
Modified transformer used as an early low-cost levitation module.
</figcaption>
</figure>

---

## Phase 2: Force Characterization

I helped design and iterate load-cell-based fixtures to measure magnetic force across current, air-gap distance, core configuration, and magnet orientation. These fixtures generated the empirical data required to determine whether candidate magnets could support the MiniPod and to provide input models for the controls team.

One transformer-based configuration produced approximately **8–9 lb of support force**, which was sufficient for the early MiniPod scale but provided limited margin for future growth.

<figure class="project-figure">
<img src="{{ '/assets/images/minipod/force-test-rigs.png' | relative_url }}">
<figcaption>
Force-characterization fixtures used to compare candidate magnets and measure force as a function of current and air gap.
</figcaption>
</figure>

---

## Phase 3: Magnetic Modeling

I used a simplified magnetic-circuit model in MATLAB to estimate flux density and attractive force before fabricating new electromagnets. The model allowed rapid comparison of:

- Core material and relative permeability
- Core diameter and length
- Number of turns
- Wire gauge
- Supplied current
- Air-gap distance

This analysis helped evaluate the central design tradeoff between coil turns and allowable current. More turns increase magnetomotive force, but typically require thinner wire with higher resistance and lower current capacity.

<figure class="project-figure">
<img src="{{ '/assets/images/minipod/matlab-magnetic-model.png' | relative_url }}">
<figcaption>
MATLAB magnetic-circuit model used to compare electromagnet geometry, core material, winding count, current, and air gap.
</figcaption>
</figure>

---

## Phase 4: Levitation Controls

The characterized magnets were then integrated into a levitation controls test rig. A distance sensor measures the magnet-to-track air gap while a PWM-controlled circuit regulates coil current for PID control.

Current work focuses on mapping magnetic force as a function of current and distance,

\[
F = F(I,z)
\]

and using that relationship to tune stable one-dimensional levitation. Testing also showed that commercial holding-force ratings can be misleading: a magnet rated near **900 lb** produced only about **20 lb at a 6 mm operating gap**.

<figure class="project-figure">
<img src="{{ '/assets/images/minipod/levitation-controls.png' | relative_url }}">
<figcaption>
Current-control circuit, force mapping, and levitation fixture used for sensor evaluation and PID tuning.
</figcaption>
</figure>

---

## Phase 5: Custom Electromagnets

As funding increased, the project transitioned from modified transformers to custom electromagnets. We developed an automated coil winder to improve repeatability and support controlled comparison of winding patterns.

Current prototypes use approximately **97–99% pure iron cores**. Ongoing optimization focuses on:

- Core geometry and cross-sectional area
- Number of turns
- Wire gauge and allowable current
- Coil density and winding pattern
- Parallel-wire configurations
- Magnetic force before thermal or saturation limits

<figure class="project-figure">
<img src="{{ '/assets/images/minipod/automatic-winder.png' | relative_url }}">
<figcaption>
Custom electromagnet produced with the team’s automated winding system.
</figcaption>
</figure>

---

## Key Engineering Tradeoffs

- **Core performance versus cost:** Higher-purity materials improve force but are more expensive and difficult to source.
- **Turns versus current:** More turns increase field strength but raise resistance and reduce allowable current.
- **Air gap versus stability:** Smaller gaps increase force but demand tighter sensing and control.
- **Holding force versus operating force:** Near-zero-gap ratings substantially overstate useful levitation performance.
- **Modeling versus testing:** MATLAB accelerated design comparisons, but saturation, leakage, and manufacturing variation required experimental validation.
- **Magnet strength versus system mass:** Larger magnets also require more structure, power, and cooling.

---

## Key Contributions

- Maintained ownership of the MiniPod from Magnetics team member through Magnetics Lead and Mechanical Lead.
- Helped establish the MiniPod as a modular levitation-development platform.
- Characterized transformer cores through B-H and force testing.
- Designed modular test rigs for current, force, and air-gap characterization.
- Developed MATLAB tools for rapid electromagnet parameter studies.
- Generated force data for closed-loop controls development.
- Supported PWM current control and PID-based levitation testing.
- Helped transition the system to custom-wound electromagnets.
- Developed an automated coil-winding process for repeatable in-house manufacturing.
- Coordinated mechanical, controls, power, manufacturing, and systems-level interfaces.

---

## Current Status

The team is completing one-dimensional levitation controls while rebuilding the MiniPod around the latest subsystem architecture. In parallel, we are refining custom electromagnet geometry, winding patterns, and core selection.

The next major milestone is a functional MiniPod using characterized custom electromagnets and stable levitation controls, followed by evaluation for eventual full-scale pod integration.

---

## Technical Skills Demonstrated

- Electromagnetic System Design
- Magnetic Circuit Modeling
- MATLAB
- Electromagnet Characterization
- Test Fixture Design
- Load Cell Instrumentation
- Automated Coil Winding
- Sensor Integration
- CAD and Mechanical Integration
- Experimental Validation
- Design Optimization
- Cross-Functional Systems Engineering


