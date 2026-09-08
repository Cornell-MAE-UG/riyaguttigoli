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

## Engineering Highlights

- Designed a custom **3-degree-of-freedom robotic testing platform** capable of independently actuating roll, pitch, and yaw motion for fiber optic strain sensors.
- Developed the complete mechanical assembly in **Onshape**, including a spherical actuator, modular sensor mounting interface, adjustable support structure, and geared yaw mechanism.
- Designed the apparatus to accommodate multiple fiber optic geometries and PCB configurations through a modular fixture architecture.
- Fabricated custom structural components using **FDM 3D printing**, laser-cut acrylic, and commercially sourced mechanical hardware.
- Integrated multiple servo motors for coordinated multi-axis motion and developed embedded control architecture using **Arduino**.
- Implemented preliminary servo control software while integrating dedicated communication hardware for Dynamixel servo control.
- Designed the platform to support future synchronized data collection between actuator position and optical sensor measurements.
- Collaborated on iterative prototyping, manufacturing, assembly, troubleshooting, and design refinement throughout multiple hardware revisions.

---

## Current Progress

The first-generation prototype successfully demonstrates the complete mechanical architecture of the testing platform, including:

- Independent roll, pitch, and yaw actuation
- Modular mounting system for different fiber optic sensor geometries
- Adjustable vertical positioning for varying specimen heights
- Integrated servo-driven motion platform
- Functional proof-of-concept hardware prototype

Current work focuses on:

- Completing embedded control software
- Integrating Dynamixel servo communication
- Automating synchronized motion sequences
- Collecting repeatable strain datasets
- Improving positioning accuracy and repeatability
- Preparing the platform for long-duration automated testing of volumetrically manufactured fiber optic sensors.

---

## Selected Figures

<figure class="project-figure">
<img src="{{ '/assets/images/orl/orl_cover.png' | relative_url }}">
<figcaption>
Complete CAD assembly of the three-degree-of-freedom testing platform showing the spherical actuator, modular specimen fixture, and independent yaw rotation mechanism.
</figcaption>
</figure>

<figure class="project-figure">
<img src="{{ '/assets/images/orl/spherical_actuator.png' | relative_url }}">
<figcaption>
Cross-sectional CAD model of the custom spherical actuator used to independently control roll and pitch motion through internally mounted servo motors.
</figcaption>
</figure>

<figure class="project-figure">
<img src="{{ '/assets/images/orl/prototype.png' | relative_url }}">
<figcaption>
First-generation physical prototype fabricated using FDM 3D printing, laser-cut acrylic, and commercial mechanical hardware for rapid design validation.
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

