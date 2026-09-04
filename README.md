# Filtered PRM* for Maps of Dynamics-Aware Motion Planning

Master's thesis, Aalto University, 2026

**Technologies:** C++, Python, OMPL, CMake, Linux, Aalto Triton HPC

## Overview

Developed and evaluated a probabilistic connection filter for the PRM*
robot motion-planning algorithm. The filter uses Maps of Dynamics (MoDs)
during roadmap construction to preferentially reject connections with high
MoD cost.

The implementation was integrated into an existing C++/OMPL research
motion-planning framework. I also developed Python workflows for running
and analysing experiments using real pedestrian tracking data.

## Results

- Reduced roadmap edge count by **32.7% on average**
- Maintained a **100% solution success rate**
- Smaller roadmaps produced only modest query-time improvements
- Filtering did not improve overall solution cost compared with regular PRM*

## Note

The thesis extended an existing research codebase that I do not have
permission to redistribute. I will add code for a demonstration of the 
filtered prm* in the future
