---
layout: project
title: "Testing Environment for Volumetric Fiber Optic Strain Sensors"
description: Designing and developing a modular three-degree-of-freedom testing environment for characterizing volumetrically manufactured fiber optic strain sensors through automated motion control, embedded systems, and integrated data acquisition.
technologies: [Onshape, Arduino, Embedded Systems, Servo Control, Mechanical Design, 3D Printing, Robotics, Systems Integration]
categories: [robotics, hardware, research]
card_tags: [Research, Robotics, Sensors]
order: 2
image: /assets/images/orl/orl_cover.png
---

## Project Overview

<img src="{{ '/assets/images/orl/orl_cover.png' | relative_url }}"
class="overview-image">

As part of my **Systems Engineering M.Eng. project** in Cornell's **Organic Robotics Laboratory**, I am developing an automated testing platform for characterizing **fiber optic strain sensors fabricated through Volumetric Additive Manufacturing (VAM)**. These soft optical sensors enable distributed strain measurement for applications including soft robotics, wearable sensing, and human-machine interfaces, but require a repeatable method of applying controlled multi-axis loading for characterization.

Working under **Professor Robert Shepherd** and PhD researcher **Hayden Webb**, I designed and continue to develop a robotic test apparatus capable of independently controlling **roll, pitch, and yaw** motion while synchronizing sensor measurements with actuator position. The platform combines custom mechanical design, embedded control, electronics integration, and automated data acquisition to generate high-quality datasets for future sensor calibration and machine learning models.

The project is currently ongoing and continues to evolve as additional sensing, control, and automation capabilities are integrated into the system.

---
## System Architecture

I developed the test environment around a modular architecture that connects the mechanical actuation, sensor fixture, embedded electronics, and data acquisition system. The platform applies controlled three-axis deformation to the fiber optic specimen while recording actuator position and optical response for sensor characterization.

<figure class="project-figure">
<img src="{{ '/assets/images/orl/functional_sketch.png' | relative_url }}">
<figcaption>
Functional architecture of the test environment, showing how the mechanical actuation, sensor interfaces, embedded control, and data acquisition systems work together to apply controlled deformation and collect synchronized measurements.
</figcaption>
</figure>

The physical architecture separates the three controlled degrees of freedom between the spherical actuator and an independent rotation mechanism. Two internal servos generate bending about the x- and y-axes, while a suspended servo and shaft assembly provide rotation about the z-axis. Modular PCB and specimen interfaces allow different fiber optic configurations to be installed without redesigning the complete apparatus.

<figure class="project-figure">
<img src="{{ '/assets/images/orl/structural_sketch.png' | relative_url }}">
<figcaption>
Structural architecture identifying the primary mechanical, actuation, sensing, and electronics components of the test platform.
</figcaption>
</figure>

---

## Engineering Highlights

-  Designed a custom **3-DOF robotic testing platform** for controlled bending and twisting of volumetrically manufactured fiber optic strain sensors.
- Developed the complete mechanical assembly in **Onshape**, including the spherical actuator, independent z-axis rotation mechanism, sensor fixtures, and supporting structure.
- Designed modular PCB and specimen interfaces to accommodate different fiber optic geometries and test configurations.
- Fabricated and iterated custom components using **FDM 3D printing**, laser-cut acrylic, and commercial hardware.
- Integrated servo-driven actuation with **Arduino-based embedded control** and dedicated Dynamixel communication hardware.
- Developed the system architecture for synchronizing commanded motion, actuator position, and optical sensor measurements for future calibration and machine-learning datasets.
- Iteratively assembled, tested, and refined the hardware as sensing and control requirements evolved.

---

### Current Progress

The first-generation prototype demonstrates the complete mechanical architecture of the platform, including independent three-axis actuation, modular sensor mounting, adjustable specimen positioning, and integrated servo-driven motion.

<figure class="project-figure">
<img src="{{ '/assets/images/orl/prototype.png' | relative_url }}">
<figcaption>
First-generation physical prototype used to validate the mechanical architecture and multi-axis actuation concept.
</figcaption>
</figure>

Current development focuses on completing embedded control, integrating position sensing and Dynamixel communication, improving motion accuracy and repeatability, and synchronizing actuator position with optical measurements for automated sensor characterization.

---

## Selected Figures

<figure class="project-figure">
<img src="{{ '/assets/images/orl/spherical_actuator.png' | relative_url }}">
<figcaption>
Cross-sectional CAD model of the custom spherical actuator used to independently control roll and pitch motion through internally mounted servo motors.
</figcaption>
</figure>


<figure class="project-figure">
<img src="{{ '/assets/images/orl/servo_closeup.png' | relative_url }}">
<figcaption>
Internal view of the spherical actuator highlighting the integrated servo transmission used for multi-axis rotational control.
</figcaption>
</figure>

---

## Ongoing Development

Future work includes:

- Closed-loop multi-axis motion control
- Automated experimental test sequences
- Synchronization of actuator position with fiber optic sensor output
- Long-duration autonomous testing
- Calibration of optical strain measurements
- Integration of machine learning models for strain estimation and sensor characterization

This project is actively under development as part of my M.Eng. research in the Organic Robotics Laboratory.

---
## Technical Skills Demonstrated

- Robotics System Design
- Mechanical Design
- Systems Integration
- Embedded Systems
- Servo Motor Control
- Arduino Programming
- CAD (Onshape)
- Rapid Prototyping
- Design for Manufacturing
- 3D Printing
- Test Automation
- Hardware Prototyping
- Mechatronics
- Experimental Design

