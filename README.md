# Project Overview

In this project we combine experimental biology and modeling to investigate the microbial community response to perturbation, and understand the role Horizontal Gene Transfer (HGT) plays in the matter. 

This repository will allow all the active members to share and sync files related to the project. 
In this wiki we will document the overall process and aims in the project.


## Aims

### Aim 1
We first aim to develop an overarching theoretical framework. We will construct a modeling framework that considers four main components: \
(1) Plastic variation in the value of a trait \
(2) Evolution \
(3) Mesoscopic structure \
(4) Environmental heterogeneity and perturbations

This will lead to a nonlinear system with analogs in physics of collective behavior. The design of our computational experiments will allow us to compare the relative contribution of different model components to emerging mesoscopic structure and stability.

Here we will ask: \
a. How is community evolution mediated by the environment? \
b. How does variation in evolved structures affect response to perturbations?

### Aim 2
Our second aim will be to investigate the response of bacterial communities to environmental change. This will be done experimantelly using a noval experimental system that grows the communities in conditions that are closer to nature - using sterilized soil media instead of lequid media which allows spatially-structured, nutrient-complex habitats. The experiment will focus on community adaptations rather than on phenotypic plasticity

Here we will ask: \
a. How do pairwise interactions in soil communities vary with environmental change? \
b. How do the evolutionary responses of communities vary with composition and environmental change?


### Aim 3
Lastly We will investigate the multilayer effect of HGT and competition on community response. Specificaly by Plasmids, and how plasmid cost vs benefit interplay between the structure of competition and HGT networks. This will be done theoretically and experimentally, in the context of response to perturbations. 



## Leading Students in the Project

* Chiara -

* [Johannes](https://johannesnauta.com)  - 
I am a postdoctoral researcher from The Netherlands who is interested in unveiling mechanisms that facilitate long-term stability of ecological systems.
In particular, I want to know how organisms respond to changes in the environment and how these responses subsequently affect ecological network dynamics.
Within the context of this project I will therefore be focusing on modeling the population dynamics of the microbiomes.
I will implement efficient simulations to explore the space of parameters that influences the community dynamics.
These explorations will then serve to define hypotheses to be tested empirically in the lab.
Furthermore, I intend to write a cohesive set of scripts that faciliate large computer simulations on high performance computer clusters.
This will make it easier for *all* members of this project to execute simulations and complex analyses, greatly enhancing the turnover rate of (simulation) experiments.
Finally, I aim to apply my knowledge on open science to accomodate efficient workflows for storing, retrieving and analysing the data associated with this project.


* Kaitlin - I am working on the experimental/lab work aspect of things. Jamie and I are creating a synthetic bacterial community comprised of 6-8 species. We will first test how the sign (+/0/-) and strength of the pairwise interactions between community members may change under different environmental conditions (e.g. increased nutrients, increasing temperature, low levels of an antibiotic, presence of mercury). We will then test how these different environmental conditions affect population dynamics of each species when all species are cultured together as a community. We will perform both experiments over both ecological (1 week) and evolutionary (~40 weeks/300 generations) time scales (In this case what we do is to set up the evolution experiment and get the ecological time scale by simply sampling those populations after one week before transferring them to the next cycle (i.e. moving them to a new culture plate with fresh media)). Next, we will perform the same pairwise and whole-community evolution experiment with an HGT component. We will do two experiments, each time introducing one of two plasmids with different properties (e.g. host ranges, genes conferring resistance to environmental stressors like antibiotics or mercury) into one bacterial strain. We will then check the effect of the plasmid on population dynamics in both the pairwise and whole-community set ups. If possible, we will also track plasmid frequencies within different species in the whole-community set up. Our overarching goal is to understand how environment shapes biotic interactions and factors that influence community robustness in the face of different types of environmental change.

* Sebastian - 

* Ying-Jie - 


## Paper Suggestions

- [N. Masuda, C.L. Vestergaard, 2022, "Gillespie algorithms for stochastic multiagent dynamics in populations and networks"](https://www.cambridge.org/core/elements/gillespie-algorithms-for-stochastic-multiagent-dynamics-in-populations-and-networks/DD6A40E1A11F3703E2807E35709B5542)  
Very thorough book about Gillespie algorithms and their uses. Also includes approaches for speeding up or reducing the memory load for Gillespie algorithms.
- [P.G. Fennel, _et al_., 2016, "Limitations of discrete-time approaches to continous-time contagion dynamics"](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.94.052125)  
Concise paper in Phys. Rev. E about why the Gillespie algorithms (and similar event-based approaches) are useful.
- [B. Morsky, D. Can Vural, 2022, "Surpressing evolution of antibiotic resistance through environmental switching"](https://link.springer.com/article/10.1007/s12080-022-00530-4)
Interesting paper on population dynamics and evolution under changing environments. They focus on similar applications as us (but do not include horizontal gene transfer) and use similar techniques as well. They use a `Julia` library called [`Catalyst.jl`](https://github.com/SciML/Catalyst.jl) which appears to be doing very similar things to our current implementations as well. The paper focuses on leveraging competition to devise a strategy of environmental switching that suppresses an infection while avoiding resistant mutants. 
