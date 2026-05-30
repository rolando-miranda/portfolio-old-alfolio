---
layout: page
title: Peristaltic Pump with Open-Loop Flow Control
description: Mechatronic peristaltic pump driven by an STM32 microcontroller, with open-loop flow control calibrated against measured flow rates.
img: assets/img/projects/peristaltic_pump_cover.jpg
importance: 2
category: mechatronics
related_publications: false
giscus_comments: false
github: https://github.com/rolomiranda98/peristaltic-pump-stm32   # CHANGE once repo exists
---

## Overview

A peristaltic pump built for NYU Tandon's Mechatronics course. The goal: deliver a target volumetric flow rate using an open-loop control strategy, characterized empirically rather than from first-principles fluid models.

## What I'm building

- **Mechanical design.** Roller head, tubing path, and motor mounting designed in SolidWorks; printed and assembled in the lab.
- **Electronics.** STM32 microcontroller driving a stepper motor through a driver board. Optical sensing for shaft position / pulse counting.
- **Firmware.** C firmware that maps a user-set flow rate to a stepper speed using a calibration curve derived from measured flow rates at known PWM duty cycles / step rates.

## Status

In progress. As of late 2025 the mechanical assembly and electronics are working; firmware and calibration are next. Updates will be posted to the linked GitHub repo as the project progresses.

## Why this is interesting

Peristaltic pumps are deceptively simple but show up everywhere in medical devices, lab automation, and bioprocessing — the open-loop control problem is realistic and the calibration approach generalizes well to similar instruments.
