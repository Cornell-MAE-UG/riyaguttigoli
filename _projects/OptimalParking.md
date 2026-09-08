---
layout: project
title: "Optimal Parking via Dynamic Programming"
description: Formulated and solved a stochastic optimal stopping problem using dynamic programming and approximate dynamic programming to determine optimal parking decisions under uncertainty.
technologies: [MATLAB, Dynamic Programming, Markov Decision Processes, Approximate Dynamic Programming, Stochastic Optimization]
categories: [modeling]
card_tags: [Dynamic Programming, Optimization]
order: 10
image: /assets/images/5680/coverpic.png
---

## Project Overview

<img src="{{ '/assets/images/5680/coverpic.png' | relative_url }}"
class="overview-image">

As part of **SYSEN 5680: Optimal Control and Decision Theory**, I formulated and solved a finite-horizon stochastic optimal stopping problem using Dynamic Programming (DP). The objective was to determine the optimal strategy for selecting a parking space when availability is uncertain and only becomes known upon arrival at each space.

The parking search was modeled as a **Markov Decision Process (MDP)** in which each parking space represented a sequential decision point. At every stage, the controller chooses whether to park immediately or continue searching, balancing the immediate walking distance against the expected benefit of finding a closer available space. I derived the Bellman recursion, implemented the optimal policy in MATLAB, and validated the resulting controller through Monte Carlo simulation.

To investigate computational tradeoffs, I also implemented a **one-step lookahead approximate dynamic programming (OSLA)** policy and compared its performance against the exact DP solution. The comparison demonstrated how reducing computational complexity can significantly degrade decision quality in stochastic optimization problems.

---

## Engineering Highlights

- Formulated the parking search problem as a finite-horizon **Markov Decision Process (MDP)** with observable state, stochastic disturbances, and binary control actions.
- Derived the Bellman optimality equations and backward recursion for the cost-to-go function.
- Implemented the exact Dynamic Programming solution in MATLAB using recursive value-function computation.
- Developed the optimal threshold-based stopping policy that minimizes expected walking distance while accounting for uncertain parking availability.
- Designed and implemented a **One-Step Lookahead Approximate Dynamic Programming (OSLA)** controller to investigate computational efficiency versus optimality.
- Performed Monte Carlo simulations to validate that the implemented DP policy converged to the analytically predicted expected cost.
- Compared exact and approximate policies through threshold analysis, expected cost evaluation, and performance bounds.
- Visualized optimal policies, value functions, stopping thresholds, and simulation results using MATLAB.

---

## Key Results

The analysis demonstrated that:

- The optimal parking strategy follows a **threshold policy**, parking only when the expected future benefit no longer outweighs the current parking opportunity.
- Under the selected parameters (**N = 100**, **p = 0.30**, **M = 25**), the optimal controller delayed parking until approximately **8 spaces from the entrance**.
- The One-Step Lookahead approximation parked substantially earlier (approximately **25 spaces from the entrance**) because it overestimated the cost of continuing.
- The exact Dynamic Programming solution achieved an expected cost of approximately **7**, while the approximate policy produced an expected cost near **21.5**.
- The approximate controller exhibited roughly a **200% higher expected cost**, illustrating the importance of accurately modeling future uncertainty in stochastic decision problems. 

---

## Selected Figures

<figure class="project-figure">
<img src="{{ '/assets/images/5680/mdp_formulation.png' | relative_url }}">
<figcaption>
Markov Decision Process formulation illustrating the system state, control actions, stochastic disturbance, and state transitions for the parking optimization problem.
</figcaption>
</figure>

<figure class="project-figure">
<img src="{{ '/assets/images/5680/optimal_policy.png' | relative_url }}">
<figcaption>
Optimal threshold policy showing the switching point between continuing to search and parking immediately when a space is available.
</figcaption>
</figure>

<figure class="project-figure">
<img src="{{ '/assets/images/5680/cost_comparison.png' | relative_url }}">
<figcaption>
Comparison of immediate parking cost and expected continuation cost used to derive the optimal stopping policy through Bellman's Principle of Optimality.
</figcaption>
</figure>

<figure class="project-figure">
<img src="{{ '/assets/images/5680/policy_comparison.png' | relative_url }}">
<figcaption>
Comparison between the exact Dynamic Programming policy and the One-Step Lookahead approximation, illustrating how limited future information shifts the stopping threshold.
</figcaption>
</figure>


---

## Technical Skills Demonstrated

- Dynamic Programming
- Approximate Dynamic Programming
- Reinforcement Learning Fundamentals
- Markov Decision Processes
- Bellman Recursion
- Stochastic Optimization
- Optimal Control
- MATLAB
- Monte Carlo Simulation
- Systems Modeling
- Mathematical Optimization

---

## Project Resources

**Full Technical Report**

[Download Project Report]({{ 'assets\reports\5680_Final_ProjectReport.pdf' | relative_url }})



**Final Presentation**

[Download Presentation]({{ 'assets\reports\SYSEN5680 Term Project_ Optimal Parking via Dynamic Programming.pdf' | relative_url }})