---
title: "Graph Neural Networks for Multi-Robot Coordination"
excerpt: "Using structured communication and learning to coordinate robot teams—going beyond simple local rules to achieve globally effective behaviors."
image: /images/research/patrolling.png
order: 1
tags:
  - graph neural networks
  - multi-robot coordination
  - learning
  - DCIST
---

**The core question:** How can locally communicating robots share structured information across the team to perform environmental monitoring more effectively?

## The Problem with Local Rules

Classical coverage control (Lloyd's algorithm) work well when robots sensor ranges can cover the entire environment. But in realistic scenarios—robots with limited sensing ranges, non-uniform starting positions, sparse regions of interest—purely local gradient-based approaches get stuck in poor configurations.

The insight: robots could do much better if they shared relevant information with each other across the network. But *what* information should they share, and *how* should they use it?

## Our Approach: Learning to Communicate

We use **Graph Neural Networks (GNNs)** to learn communication policies that allow robots to leverage non-local information while remaining fully decentralized:

- Each robot computes local gradient information from its sensors
- The GNN transforms and propagates this information through the communication network
- Multi-hop communication allows robots to "see" beyond their immediate neighbors
- The policy is trained via imitation learning from a clairvoyant expert

The GNN architecture naturally handles the permutation symmetry in robot teams and scales gracefully to larger teams than seen during training.

## Key Results

- **Significantly higher coverage quality** compared to Lloyd's algorithm on challenging non-uniform coverage densities
- **Transfers to new scenarios**: policies trained on one density distribution work on others
- **Scales to larger teams**: 10-robot policies work on 20+ robot teams
- **Explicit communication benefit**: ablation studies confirm the value of multi-hop information sharing

## Publications

- **IEEE International Conference on Robotics and Automation (ICRA), 2022**  
  *Coverage Control in Multi-Robot Systems via Graph Neural Networks*  
  W. Gosrich, S. Mayya, R. Li, J. Paulos, M. Yim, A. Ribeiro, V. Kumar  
  [arXiv](https://arxiv.org/abs/2109.15278) &#124; [IEEE](https://ieeexplore.ieee.org/document/9812335)

## Collaborators

This work was conducted at Penn's GRASP Lab as part of the [DCIST](https://dcist.org) program.
