# Filtered-PRM-for-MoDs-aware-Motion-Plannning
DEMO CODE COMING SOON

My Aalto university master's thesis

Technologies used: C++, Python, OMPL, CMake, Linux, Aalto Triton HPC 

## My contributions

- Developed and evaluated a probabilistic connection-filtering approach for the PRM* robot motion-planning algorithm, using Maps of Dynamics to influence roadmap construction.
- Implemented the proposed filtering method in an existing C++/OMPL motion-planning framework.
- Developed experimental and analysis workflows using Python. Designed experiments used real pedestrian tracking data to compare path quality markers and simulated interference with people.

## Results
- Reduced the number of roadmap edges by 32.7% on average while retaining a 100% solution success rate across the tested conditions.
- Showed that smaller roadmaps provided only modest query-time improvements and did not improve overall solution cost.

## Abstract 
Successful deployment of mobile robots in human environments requires motion 
planning methods that account for the common human motion patterns in that 
environment. Maps of Dynamics (MoDs) are able to capture such motion patterns 
learned from observations. This information can be integrated into motion 
planners to guide robots toward paths that better conform to the environment. 

The objective of this thesis is to study whether MoD-aware probabilistic roadmap 
planning (PRM*) can be improved by utilizing MoD information during roadmap 
construction. A probabilistic MoD-informed connection filter is proposed which 
rejects candidate connections with high MoD costs with a higher probability. The 
motivation for this is to reduce the number of less desirable connections and 
thereby improve query efficiency and solution quality. The experimental setup 
includes intensity, GMMT, and CLiFF MoD representations, and the MoD-filtered 
PRM* is compared to regular MoD-informed PRM* and a baseline randomly 
filtered PRM*. The experiments use pedestrian tracking data collected from a 
shopping center and evaluate roadmap size, query time, solution cost, success rate, 
and simulated interference with people. 

The proposed filter was successful in reducing the number of edges in the roadmap 
while maintaining a 100% success rate. However, the total solution cost increased 
for all  three MoD representations at matched query times. The baseline random 
filter also outperformed the MoD-filter in terms of total cost. The interference 
results were more mixed as intensity-based filtering produced a small reduction in 
interference, whereas GMMT and CLiFF filtering did not provide a consistent 
advantage. These results tell us that the proposed MoD-aware filter did not improve 
MoD-informed PRM*. Future filtering methods should also account for the global 
structural importance of each connection. 
