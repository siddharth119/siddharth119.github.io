---
title: "Resilience in Heterogeneous Multi-Robot Systems"
excerpt: "How do you keep a robot team working effectively when things go wrong? Algorithms that assign the right robots to the right tasks—and adapt when robots fail or conditions change."
image: /images/research/hetero_res.jpg
order: 2
tags:
  - task allocation
  - heterogeneous robots
  - resilience
  - DCIST
---

## The Challenge

Heterogeneity in robot capabilities--different sensors, different morphologies--can contribute favorably to several aspects of multi-robot operations, include *resilience* which is defined as the ability of the system to react to component failures, adversarial attacks, and varying environmental conditions. However acheiving resilience over long-duration deployments of robot systems in dynamic environments is an open challenge in robobitcs.

As part of multiple projects at UPenn and Georgia Tech, I've worked on modeling the heterogeneous capabilities of robots and leveraging hierarchical optimization frameworks for a coordinated approach between task allocation and task execution -- with the ultimate goal of imparting resilience in these multi-robot systems.

## Our Approach

We developed algorithms that explicitly reason about **which robots are essential** and **what risks are worth taking**:

**Feature-Capability Framework**: We model what each robot *can do* based on its sensors and actuators. When a robot fails, the system automatically finds backups—if Robot A's camera breaks, maybe Robot B's LIDAR can fill in.

**Adaptive Risk Management**: In adversarial settings, we've built algorithms that track a "sensing margin"—how much redundancy the team has. With plenty of backup, robots can be aggressive. As failures accumulate, survivors automatically become conservative to preserve remaining capability.

**Energy-Aware Allocation**: For long missions, we minimize energy while meeting task requirements—continuously re-evaluating whether to send a distant but capable robot or use a nearby but less capable one.

**Task Precedence and Cooperation**: Recent work extends this to missions with complex task dependencies, using network flow algorithms to efficiently form coalitions while respecting precedence constraints.

## Publications

- **IEEE Transactions on Robotics (T-RO), 2025**  
  *Online Multi-Robot Coordination with Task Precedence Relationships*  
  W. Gosrich, S. Agarwal, K. Garg, S. Mayya, M. Malencia, M. Yim, V. Kumar  
  [arXiv](https://arxiv.org/abs/2509.15052)

- **IEEE Transactions on Robotics (T-RO), 2021**  
  *A Resilient and Energy-Aware Task Allocation Framework for Heterogeneous Multi-Robot Systems*  
  G. Notomista, S. Mayya, Y. Emam, C. Kroninger, A. Bohannon, S. Hutchinson, M. Egerstedt  
  [arXiv](https://arxiv.org/abs/2105.05586) &#124; [IEEE](https://ieeexplore.ieee.org/document/9524493)

- **IEEE Robotics and Automation Letters (RA-L), 2022**  
  *Adaptive and Risk-Aware Target Tracking for Robot Teams with Heterogeneous Sensors*  
  S. Mayya, R.K. Ramachandran, L. Zhou, V. Senthil, D. Thakur, G.S. Sukhatme, V. Kumar  
  [arXiv](https://arxiv.org/abs/2105.03813) &#124; [IEEE](https://ieeexplore.ieee.org/document/9681233)

- **IEEE Robotics and Automation Letters (RA-L), 2021**  
  *Resilient Active Target Tracking with Multiple Robots*  
  S. Mayya, P. Tokekar, V. Kumar  
  [arXiv](https://arxiv.org/abs/2001.04099) &#124; [IEEE](https://ieeexplore.ieee.org/abstract/document/9349130)

- **IEEE International Conference on Robotics and Automation (ICRA), 2020**  
  *Adaptive Task Allocation for Heterogeneous Multi-Robot Teams with Evolving and Unknown Robot Capabilities*  
  Y. Emam, S. Mayya, G. Notomista, A. Bohannon, M. Egerstedt  
  [arXiv](https://arxiv.org/abs/2003.03344) &#124; [IEEE](https://ieeexplore.ieee.org/document/9196627)

## Videos

<div class="video-grid">
  <div class="video-item">
    <iframe src="https://www.youtube.com/embed/TRceQUiTnik" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
  <div class="video-item">
    <iframe src="https://www.youtube.com/embed/fdfYID7u72o" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
</div>

<div class="video-grid">
  <div class="video-item">
    <iframe src="https://www.youtube.com/embed/EpcmsUVGlgw" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
</div>

## Collaborators

Part of the [DCIST](https://dcist.org) program with Georgia Tech, USC, and ARL.
