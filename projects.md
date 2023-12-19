---
layout: archive
title: ""
permalink: /projects/
author_profile: true
redirect_from:
  - /projects
---

# <u>Air Traffic Control Problem</u> <font size=4>[<a href="https://jamesarambam.github.io/files/icaps21.pdf">ICAPS-2021</a>]</font>

Many real world systems involve interaction among large number of agents to achieve a common goal, for example, air traffic control. Several model-free RL algorithms have been proposed for such settings. A key limitation is that the empirical reward signal in model-free case is not very effective in addressing the multiagent credit assignment problem, which determines an agent's contribution to the team's success. This results in lower solution quality and high sample complexity. To address this, we contribute (a) an approach to learn a differentiable reward model for both continuous and discrete action setting by exploiting the collective nature of interactions among agents, a feature commonly present in large scale multiagent applications; (b) a shaped reward model analytically derived from the learned reward model to address the key challenge of credit assignment; (c) a model-based multiagent RL approach that integrates shaped rewards into well known RL algorithms such as policy gradient, soft-actor critic. Compared to previous methods, our learned reward models are more accurate, and our approaches achieve better solution quality on synthetic and real world instances of  air traffic control, and cooperative navigation with large agent population.

<img src="https://jamesarambam.github.io/images/london3.png" alt="drawing" width="600" height="200"/>

# <u>Maritime Traffic Management Problem</u><font size=4> [<a href="https://www.aaai.org/ojs/index.php/AAAI/article/view/4575">AAAI-19</a>, <a href="http://ifaamas.org/Proceedings/aamas2020/pdfs/p1278.pdf">AAMAS-20</a>]</font>

We address the problem of maritime traffic management in busy waterways to increase the safety of navigation by reducing congestion. We model maritime traffic as a large multiagent systems with individual vessels as agents, and the port authority as the regulatory agent. We develop a maritime traffic simulator based on historical traffic data that incorporates realistic domain constraints such as uncertain and asynchronous movement of vessels. We also develop a traffic coordination approach that provides speed recommendation to vessels in different zones. We exploit the nature of collective interactions among agents to develop a scalable policy gradient approach that can scale up to real world problems. Empirical results on synthetic and real world problems show that our approach can significantly reduce congestion while keeping the traffic throughput high.

<img src="https://jamesarambam.github.io/images/enc.png" alt="drawing" width="600" height="200"/>

# <u>Graph Based Optimization For Multiagent Cooperation</u> <font size=4>[<a href="https://dl.acm.org/doi/10.5555/3306127.3331863">AAMAS-19</a>]</font>

We address the problem of solving math programs defined over a graph where nodes represent agents and edges represent interaction among agents. The objective and constraint functions of this program model the task agent team must perform and the domain constraints. In this multiagent setting, no single agent observes the complete objective and all the constraints of the program. Thus, we develop a distributed message-passing approach to solve this optimization problem. We focus on the class of graph structured linear and quadratic programs (LPs/QPs) which can model important multiagent coordination frameworks such as distributed constraint optimization (DCOP). For DCOPs, our framework models functional constraints among agents (e.g. resource, network flow constraints) in a much more tractable fashion than previous approaches. Our iterative approach has several desirable properties—it is guaranteed to find the optimal solution for LPs, converges for general cyclic graphs, and is memory efficient making it suitable for resource limited agents, and has anytime property. Empirically, our approach provides solid empirical results on several standard benchmark problems when compared against previous approaches.

<img src="https://jamesarambam.github.io/images/agv.png" alt="drawing" width="600" height="200"/>

# <u>Decision Making For Computational Sustainability</u> <font size=4>[<a href="https://www.aaai.org/ocs/index.php/AAAI/AAAI16/paper/view/12224">AAAI-16</a>]</font>

We address the problem of robust decision making for stochastic network design. Our work is motivated by spatial conservation planning where the goal is to take management decisions within a fixed budget to maximize the expected spread of a population of species over a network of land parcels. Most previous work for this problem assumes that accurate estimates of different network parameters (edge activation probabilities, habitat suitability scores) are available, which is an unrealistic assumption. To address this shortcoming, we assume that network parameters are only partially known, specified via interval bounds. We then develop a decision making approach that computes the solution with minimax regret. We provide new theoretical results regarding the structure of the minmax regret solution which help develop a computationally efficient approach. Empirically, we show that previous approaches that work on point estimates of network parameters result in high regret on several standard benchmarks, while our approach provides significantly more robust solutions.

<img src="https://jamesarambam.github.io/images/birds.png" alt="drawing" width="500" height="150"/>


# <u>Master's Thesis: Exploration and Realtime Mapping of an Obstacle-Prone Unknown Environment Using Swarm of Autonomous Mobile Robots</u>

In my Master's thesis, I worked on research concerning the application of Swarm Robotics for mapping an unknown area with unknown obstacles. The problem of mapping an unknown environment by a swarm of mobile robots is further divided into two classic problems of Multi-Robot Systems as Multi Robot Area Partitioning Problem and Area Exploration Problem. The robots considered here follow the basic Observe-Compute-Move model, which is also known as the CORDA Model. The robots are assumed to be a full compass and asynchronous timing models, and all of them remain active throughout the process. The robots considered here are all identical, with limited visibility and limited communication. There is no centralized control. Each robot executes the same algorithm in every cycle based on the local information. We solve the mapping problem in two modules. We propose a distributed algorithm for each module and also use concepts from computational geometry. In the first module, we solve the area partitioning problem where we divide the unknown area among the robots and assign each robot a part of the area. In the second module, each robot performs an exploration of the area assigned and simultaneously generates a topological graph(map) of the sub-area. Thus, by combining graphs of all sub-parts of the area, we get a map of the area. We simulate our proposed system with Player/Stage, and the map is constructed using Python’s graphics library.


Software Simulation | Hardware Test
:-: | :-:
<video width="320" height="350" controls> <source src="https://jamesarambam.github.io/files/soft.mp4" type="video/mp4"></video> | <video width="320" height="350" controls> <source src="https://jamesarambam.github.io/files/hard_low.mp4" type="video/mp4"></video>



