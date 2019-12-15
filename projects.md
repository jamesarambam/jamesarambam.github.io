---
layout: archive
title: ""
permalink: /projects/
author_profile: true
redirect_from:
  - /projects
---


# <u>Maritime Traffic Management Problem</u> 
We address the problem of maritime traffic management in busy waterways to increase the safety of navigation by reducing congestion. We model maritime traffic as a large multiagent systems with individual vessels as agents, and the port authority as the regulatory agent. We develop a maritime traffic simulator based on historical traffic data that incorporates realistic domain constraints such as uncertain and asynchronous movement of vessels. We also develop a traffic coordination approach that provides speed recommendation to vessels in different zones. We exploit the nature of collective interactions among agents to develop a scalable policy gradient approach that can scale up to real world problems. Empirical results on synthetic and real world problems show that our approach can significantly reduce congestion while keeping the traffic throughput high.

<img src="https://jamesarambam.github.io/images/enc.png" alt="drawing" width="600" height="200"/>

# <u>Graph Based Optimization For Multiagent Cooperation</u>

We address the problem of solving math programs defined over a graph where nodes represent agents and edges represent interaction among agents. The objective and constraint functions of this program model the task agent team must perform and the domain constraints. In this multiagent setting, no single agent observes the complete objective and all the constraints of the program. Thus, we develop a distributed message-passing approach to solve this optimization problem. We focus on the class of graph structured linear and quadratic programs (LPs/QPs) which can model important multiagent coordination frameworks such as distributed constraint optimization (DCOP). For DCOPs, our framework models functional constraints among agents (e.g. resource, network flow constraints) in a much more tractable fashion than previous approaches. Our iterative approach has several desirable properties—it is guaranteed to find the optimal solution for LPs, converges for general cyclic graphs, and is memory efficient making it suitable for resource limited agents, and has anytime property. Empirically, our approach provides solid empirical results on several standard benchmark problems when compared against previous approaches.

<img src="https://jamesarambam.github.io/images/agv.png" alt="drawing" width="600" height="200"/>

# <u>Robust Decision Making For Stochastic Network Design</u>

We address the problem of robust decision making for stochastic network design. Our work is motivated by spatial conservation planning where the goal is to take management decisions within a fixed budget to maximize the expected spread of a population of species over a network of land parcels. Most previous work for this problem assumes that accurate estimates of different network parameters (edge activation probabilities, habitat suitability scores) are available, which is an unrealistic assumption. To address this shortcoming, we assume that network parameters are only partially known, specified via interval bounds. We then develop a decision making approach that computes the solution with minimax regret. We provide new theoretical results regarding the structure of the minmax regret solution which help develop a computationally efficient approach. Empirically, we show that previous approaches that work on point estimates of network parameters result in high regret on several standard benchmarks, while our approach provides significantly more robust solutions.