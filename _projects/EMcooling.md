---
layout: project
title: "Cornell Hyperloop: Electromagnet Thermal Management System"
description: Designed, experimentally validated, and implemented an active air-cooling system for off-the-shelf electromagnets, combining thermal modeling, CAD design, and hardware testing to prevent overheating during sustained operation.
technologies: [MATLAB, SolidWorks, Heat Transfer, Thermal Analysis, Mechanical Design, Experimental Testing]
categories: [hardware, modeling]
card_tags: [Thermal, Hardware, MATLAB]
order: 3
image: /assets/images/emcooling/coverpic.png
---

## Project Overview

<img src="{{ '/assets/images/emcooling/coverpic.png' | relative_url }}"
class="overview-image">

One of my first projects on Cornell Hyperloop's Magnetics Team was designing a cooling subsystem for off-the-shelf electromagnets the team was using to levitate the pod at the time. The locations of the four magnets within the pod chassis were already fixed, and my objective was to design a cooling solution around that existing architecture.

A major challenge early in the project was uncertainty. The magnets had manufacturer specifications, but we did not know how quickly they would heat under our operating conditions or whether active cooling would even be necessary. Before designing hardware, I first estimated the magnets' thermal behavior using MATLAB and researched cooling strategies used in automotive and computer systems.

The resulting subsystem used forced-air cooling with aluminum heat sinks, high-flow axial fans, and a lightweight structural mounting assembly that integrated directly into the Hyperloop chassis.

---

## Engineering Approach

Before I began the design process, I had to answer several questions: 
- How hot would the electromagnets become during operation?
- Would passive cooling be sufficient, or would active cooling be required?
- Should the system use liquid cooling or forced-air cooling?
- How could cooling hardware fit within the existing pod packaging?

Using the electromagnet specifications together with estimated operating currents, I developed a rough MATLAB model to approximate heat generation and temperature rise. While the model relied on simplifying assumptions and uncertain operating conditions, it established an expected operating range that informed the remainder of the design process.

<figure class="project-figure">
<img src="{{ '/assets/images/emcooling/matlab-model.png' | relative_url }}">
<figcaption>
MATLAB model estimating electromagnet temperature rise from electrical power dissipation.
</figcaption>
</figure>

---

## System Design

Based on the thermal estimates and available packaging volume, I selected an air-cooled architecture over liquid cooling due to its simplicity, lower cost, reduced mass, and easier integration.

The final subsystem consisted of:
- Cylindrical aluminum heat sinks surrounding each electromagnet
- 200 CFM axial fans positioned above the magnets
- A custom 3D-printed Onyx truss with heat-set inserts
- Aluminum crossbars allowing the entire assembly to be installed and serviced as a removable module

The final design also incorporated ducting concepts to draw cooler ambient air from outside the aeroshell toward the magnets during operation, but this was added later as a reinforcement measure to ensure the system wouldn't cycle hot air onto the magnets. 

<figure class="project-figure">
<img src="{{ '/assets/images/emcooling/system-cad.png' | relative_url }}">
<figcaption>
Final cooling subsystem integrating heat sinks, fan assembly, and removable mounting structure within the Hyperloop chassis.
</figcaption>
</figure>

<figure class="project-figure">
<img src="{{ '/assets/images/emcooling/insert-pic.png' | relative_url }}">
<figcaption>
Custom 3D-printed truss designed to interface with aluminum crossbars using heat-set inserts.
</figcaption>
</figure>

---

## Thermal Validation

Because the analytical model contained uncertainty, I built a benchtop test setup to experimentally evaluate the cooling concept.

A heated aluminum test article represented the electromagnet while production heat sinks and fans were arranged in their intended configuration. Using thermistors and temperature measurements over time, I evaluated cooling performance under varying airflow conditions and compared the results against analytical predictions.

<figure class="project-figure">
<img src="{{ '/assets/images/emcooling/testing.png' | relative_url }}">
<figcaption>
Experimental setup used to evaluate cooling performance and validate thermal assumptions.
</figcaption>
</figure>

---

## Results & Design Impact

The project produced Cornell Hyperloop's first dedicated thermal management subsystem for the electromagnets and proved that an actively cooled air-based solution could satisfy the team's thermal and packaging requirements for the system parameters at the time (those have since changed).

The project established an engineering workflow that combined analytical modeling, hardware prototyping, and testing to reduce uncertainty before subsystem integration. It also provided a modular, serviceable design that could be removed independently from the chassis for maintenance or future design iterations.

---

## Technical Skills Demonstrated

- Thermal Systems Engineering
- Heat Transfer
- MATLAB Modeling
- Engineering Trade Studies
- Mechanical CAD (SolidWorks)
- Design for Integration
- Experimental Testing
- Hardware Validation
- Technical Research
- Mechanical System Design