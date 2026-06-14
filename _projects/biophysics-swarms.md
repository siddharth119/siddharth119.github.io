---
title: "Biophysics-Inspired Robot Swarms"
excerpt: "Using ideas from biology and statistical mechanics to enable swarm robot behaviors leveraging local encounters as a source of information."
image: /images/research/encs.png
order: 3
tags:
  - swarm robotics
  - mean-field theory
  - statistical mechanics
  - encounters
---

**The core question:** In a dense swarm of simple robots with no explicit communication, how can individual robots infer global properties of the swarm—and use that information to coordinate?

## The Insight: Local Encounters as Information

When you pack many robots into a space, they inevitably bump into each other. Rather than treating collisions as a nuisance to avoid, we asked: **what information do these local encounters carry?**

It turns out, quite a lot. The rate at which a robot encounters other robots encodes information about local robot density. And through the lens of statistical mechanics, individual robots can use encounter statistics to estimate global swarm properties—without any explicit communication.

## Contributions

Given a swarm of minimally-equipped robots with only a proximity sensor which indicates whether another robot is near it or not, we explored the following swarm robotics applications.

- **Encounter-based localization**: Robots estimate their position in an environment by counting encounters and leveraging the kinetic theory of gases to estimate densities in various parts of the environment.
- **Task allocation without communication**: Robots switch between tasks based on encounter statistics, achieving swarm-level division of labor.
- **Density Control**: A decentralized algorithm that enables individual robots to decide whether to stay in the region and contribute to the overall mission, or vacate the region so as to reduce the negative effects that interference has on the overall efficiency of the swarm.

The mathematics draws from kinetic theory and statistical mechanics, but the algorithms are simple enough to run on tiny robots with minimal computation.

## Publications

- **IEEE Transactions on Robotics (T-RO), 2019**  
  *Localization in Densely Packed Swarms Using Interrobot Collisions as a Sensing Modality*  
  S. Mayya, P. Pierpaoli, G. Nair, M. Egerstedt  
  [IEEE](https://ieeexplore.ieee.org/document/8485322)

- **Robotics: Science and Systems (RSS), 2017**  
  *Collisions as Information Sources in Densely Packed Multi-Robot Systems Under Mean-Field Approximations*  
  S. Mayya, P. Pierpaoli, G. Nair, M. Egerstedt  
  [RSS](http://www.roboticsproceedings.org/rss13/p44.html)

- **Swarm Intelligence Journal, 2019**  
  *Closed-Loop Task Allocation in Robot Swarms Using Inter-Robot Encounters*  
  S. Mayya, S. Wilson, M. Egerstedt  
  [Springer](https://link.springer.com/article/10.1007/s11721-019-00166-x)

- **IEEE International Conference on Robotics and Automation (ICRA), 2019**  
  *Voluntary Retreat for Decentralized Interference Reduction in Robot Swarms*  
  S. Mayya, P. Pierpaoli, M. Egerstedt  
  [IEEE](https://ieeexplore.ieee.org/abstract/document/8794124)

- **IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2019**  
  *Non-Uniform Robot Densities in Vibration Driven Swarms Using Phase Separation Theory*  
  S. Mayya, G. Notomista, D. Shell, S. Hutchinson, M. Egerstedt  
  [IEEE](https://ieeexplore.ieee.org/abstract/document/8967985)

- **IEEE Multi-Robot and Multi-Agent Systems (MRS), 2019**  
  *Decentralized Minimum-Energy Coverage Control for Time-Varying Density Functions*  
  M. Santos, S. Mayya, G. Notomista, M. Egerstedt  
  [IEEE](https://ieeexplore.ieee.org/abstract/document/8901076)

- **PhD Thesis, Georgia Institute of Technology, 2019**  
  *Local Encounters in Robot Swarms: from Localization to Density Regulation*  
  S. Mayya  
  [Georgia Tech](https://smartech.gatech.edu/handle/1853/62343)

## Videos

<div class="video-grid">
  <div class="video-item">
    <iframe src="https://www.youtube.com/embed/sV7IyjpsY38" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
  <div class="video-item">
    <iframe src="https://www.youtube.com/embed/g-SroIf5_vg" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
</div>

<div class="video-grid">
  <div class="video-item">
    <iframe src="https://www.youtube.com/embed/tCoQpderrMs" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
  <div class="video-item">
    <iframe src="https://www.youtube.com/embed/SXCaT6-hwdI" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
</div>
