---
layout: project
title: "Wind Turbine Blade Design & Testing"
description: Team-based design and experimental validation of a horizontal-axis wind turbine blade through fabrication, wind tunnel testing, and performance analysis.
technologies: [MATLAB, CAD (Autodesk Inventor), BEM Theory, Wind Tunnel Testing]
categories: [energy, hardware]
card_tags: [Energy, Testing, Aerodynamics]
order: 8
image: /assets/images/4272cover.jpg
---

## Project Overview

<img src="{{ page.image | relative_url }}"
     alt="{{ page.title }}"
     class="overview-image">

As part of MAE 4272: Fluids and Heat Transfer Laboratory, our team designed, manufactured, and tested a small-scale wind turbine blade intended to maximize power extraction in Cornell’s Big Blue wind tunnel. Our objective was to apply Blade Element Momentum (BEM) theory to design an aerodynamically efficient rotor within strict geometric and experimental constraints, and then validate its real world performance through controlled wind-tunnel testing.

This project involved all elements of an engineering design process, from theoretical modeling and CAD to experimental validation and failure analysis.

---

## Design Process

We designed a three-bladed rotor using a NACA 4412 airfoil, selected for its favorable lift-to-drag characteristics at the low Reynolds numbers relevant to wind-tunnel testing. Using a custom MATLAB BEM implementation, we optimized spanwise chord and twist distributions for a target tip-speed ratio of **λ = 7** and an intended operating wind speed of approximately **5.36 m/s**.

The model predicted a peak power output of roughly **3.1 W** at **~2866 RPM**, while remaining within the torque limits of the magnetic particle brake. Structural checks were performed in MATLAB using spanwise load integration to estimate root bending stress, which initially suggested a comfortable safety factor. The final blade geometry was generated in CAD and 3D-printed for experimental testing.
<figure class="project-figure">
  <img src="{{ '/assets/images/4272pic1.png' | relative_url }}" alt="Wind turbine blade CAD geometry">
  <figcaption>Final blade geometry generated from BEM-optimized chord and twist distributions.</figcaption>
</figure>


---

## Testing Summary

<figure class="project-figure">
  <img src="{{ '/assets/images/4272pic2.jpg' | relative_url }}"
     style="max-width: 300px; display: block; margin: 1.5rem auto;">
  <figcaption>Torque-controlled wind tunnel testing setup used to characterize blade performance.</figcaption>
</figure>

The blade was tested in the Big Blue wind tunnel using a torque-controlled experimental method. Rather than prescribing RPM, we incrementally increased magnetic particle brake torque and allowed the rotor to settle naturally into steady-state rotational speeds. This approach avoided brake hysteresis effects and enables direct measurement of torque–speed and power behavior.
<figure class="project-figure">
  <img src="{{ '/assets/images/4272pic3.png' | relative_url }}"
     style="max-width: 300px; display: block; margin: 1.5rem auto;">
  <figcaption>Measured rotor power versus rotational speed at hub heights of 9 m and 10 m</figcaption>
</figure>
In practice, the printed blade struggled to self-start and required elevated tunnel speeds and manual spin-up. The rotor also stalled rapidly under load, limiting us to only 3–5 usable data points per wind speed. One blade ultimately failed structurally at the hub during testing, preventing further data collection. These results highlighted a critical disconnect between aerodynamic optimization and manufacturability-driven structural limitations.

---

## My Contribution

I contributed primarily to the aerodynamic modeling and experimental analysis aspects of the project. This included developing and validating the MATLAB BEM code, estimating power, torque, and structural loads, helping design the torque-controlled testing procedure, and analyzing discrepancies between predicted and measured performance. I also supported failure analysis and helped synthesize design lessons for future iterations.
