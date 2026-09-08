---
layout: project
title: "Cornell Hyperloop: Linear Induction Motor Thrust Characterization"
description: Experimentally characterized an off-the-shelf linear induction motor to determine whether it could propel the team’s heavy pod and inform future propulsion design decisions.
technologies: [Load Cell Testing, Test Fixture Design, Linear Induction Motors, Data Analysis, Electromechanical Testing, Systems Engineering]
categories: [hardware, research]
card_tags: [Testing, Electromagnetics, Hardware]
order: 4
image: /assets/images/lim/coverpic.png
---

## Project Overview

<img src="{{ '/assets/images/lim/coverpic.png' | relative_url }}"
class="overview-image">

As part of **Cornell Hyperloop**, I worked on the experimental characterization of a linear induction motor that had been purchased years earlier but had never been fully tested. The objective was to determine whether the motor could generate enough thrust to propel the team’s approximately **150 lb steel-chassis pod**.

I helped to develop a propulsion test setup in which the powered LIM remained fixed above an aluminum I-beam mounted on a translating rail. As the motor accelerated the beam, it contacted a load cell at the end of the fixture, allowing thrust to be measured while varying the electrical input and operating frequency.

Testing showed that thrust plateaued near **15 lb**, indicating that the motor did not provide sufficient propulsion margin for the existing vehicle. The result supported the team’s transition to a lighter aluminum chassis and motivated development of a custom LIM better matched to the pod’s geometry, mass, and power system.

---

## Experimental Setup

The test fixture isolated the LIM from the full pod so its thrust could be measured directly.

- The LIM was fixed above the aluminum I-beam secondary.
- The I-beam translated along a guided rail.
- A load cell measured the generated thrust.
- Frequency, voltage, and current were varied to evaluate performance.
- The setup allowed the motor to be assessed before full-system integration.

<figure class="project-figure">
<img src="{{ '/assets/images/lim/propulsion-test-ring.png' | relative_url }}">
<figcaption>
Early schematic of propulsion test fixture with the LIM fixed above a translating aluminum I-beam and a load cell used to measure thrust.
</figcaption>
</figure>

<figure class="project-figure">
<img src="{{ '/assets/images/lim/limpic.png' | relative_url }}">
<figcaption>
LIM full experimental test setup including power systems and makeshift faraday cages to prevent EMI. 
</figcaption>
</figure>

<figure class="project-figure">
  <video controls playsinline preload="metadata">
    <source src="{{ '/assets/videos/lim-thrust-test.mp4' | relative_url }}"
            type="video/mp4">
    Your browser does not support embedded video.
  </video>

  <figcaption>
    Experimental test showing the LIM driving the aluminum I-beam forward and backward along the rail.
  </figcaption>
</figure>

---

## Results and Design Impact

Measured thrust increased with frequency before reaching a maximum of approximately **15 lb** under the available power-system constraints.

<figure class="project-figure">
<img src="{{ '/assets/images/lim/thrust-frequency-results.png' | relative_url }}">
<figcaption>
Measured thrust across operating frequency, showing a maximum output near 15 lb.
</figcaption>
</figure>

The results showed that the purchased LIM was not well matched to the mass of the existing pod and informed several team decisions:

- Replace the steel chassis with a lighter aluminum design.
- Reevaluate the propulsion system at the full-vehicle level.
- Begin development of a custom LIM tailored to the team’s requirements.
- Account for propulsion-related electromagnetic interference during integration.

---

## Next Steps

The experimental results led to the foundation of the **Mini-LIM** project, an effort to design and manufacture a small-scale custom linear induction motor optimized specifically for Cornell Hyperloop's vehicle, power system, and packaging constraints.

Since then, the team has completed extensive research and simulation, electromagnetic design optimization, finalized key motor parameters, begun designing the stator and mounting hardware, and started preparing components for fabrication and assembly. The next phase focuses on manufacturing the stator, winding the coils, assembling the motor, and experimentally characterizing its thrust to validate the design.

I was not directly involved in the Mini-LIM design effort, but I continued overseeing its progression as Mechanical Lead while the magnetics team advanced the project toward a fully custom propulsion system.
