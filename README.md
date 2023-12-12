
# Crowd-Bridge Dynamic Interaction Simulation with Duhamel's Integral

This code simulates the dynamic response of a lively footbridge to excitation forces induced by a crowd of walking pedestrians.

## Overview

The core modeling components are:

- Simple beam bridge modeled with key modal properties - frequency, mass, damping
- Walking pedestrians, each crossing the bridge with random parameters 
  - Weight, pacing frequency and variability, crossing speed
- Pedestrian-induced forces calculated at each time step based on intrinsic weight and pacing
  - Mapped spatially to bridge mode shape
- Bridge response obtained by numerical integration of equation of motion
  - Using Duhamel's integral formulation 
- Animation shows bridge vibrating in response to cumulative pedestrian forcing

This captures the phenomenon of human structure interaction arising from lively pedestrian paces synchronizing with and exciting bridge resonance.

## Usage

The simulation allows controlling parameters like:

- Number of pedestrians crossing simultaneously
- Bridge frequency and damping ratio  
- Mean and variability of pedestrian pacing frequencies

Sample output plots and animations are saved to view the bridge acceleration response spectrum and see the mode shape deflecting in real-time.

## Potential Extensions

Future work possibilities include:

- Incorporate other lower order bridge modes and multi-mode participation
- Enable two-way human response to perceived bridge motion 
- Expand beyond deterministic to probabilistic pedestrian forcing models
- Develop vertical/lateral coupled bridge formulations
- Optimize numerical integrations for faster performance
