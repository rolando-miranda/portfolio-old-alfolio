---
layout: page
title: Autonomous Mars Rover (MuJoCo)
description: Planning and control algorithm for soil-sample collection, tested in the MuJoCo physics simulator.
img: assets/img/projects/mars_rover_cover.jpg
importance: 1
category: robotics
related_publications: false
giscus_comments: false
github: https://github.com/rolomiranda98/mars-rover-mujoco   # CHANGE once repo exists
---

## Overview

A simulated autonomous rover that locates, approaches, and collects soil samples on uneven terrain. The project combined **path planning, low-level control, and dynamics simulation** in MuJoCo, with the goal of producing a system that could handle terrain variability without hand-tuned trajectories.

## What I built

- **Planning layer.** A high-level planner that proposes candidate sample sites and orders them by accessibility, considering slope and rover heading.
- **Control layer.** Trajectory following with feedback control on heading and velocity, tuned against the rover's simulated dynamics.
- **Simulation environment.** A MuJoCo scene with the rover model, terrain, and sample targets, used to evaluate planning and control end-to-end.

## What I learned

- How planner assumptions propagate into controller failures — particularly when terrain assumptions break down at the boundary between high- and low-level layers.
- Practical limits of open-loop trajectory generation on uneven terrain, and where closed-loop correction has to step in.
- Trade-offs between simulation fidelity and iteration speed.

## Status

Completed as part of NYU Tandon coursework. Repository linked above; see the README for setup and reproduction steps.
