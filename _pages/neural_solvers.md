---
permalink: /neural_solvers/
title: ""
author_profile: true
redirect_from:
  - /pinn/
  - /neural_solvers.html
---

![Drag Racing](https://raw.githubusercontent.com/Photon-AI-Research/NeuralSolvers/master/images/cropped_logo.png)

Neural Solvers are neural network based solver for partial differential equations and inverse problems. 
Our library [Neural Solvers](https://github.com/Photon-AI-Research/NeuralSolvers) implements the physics-informed neural network approach on scale. Physics informed neural networks allow strong scaling by design. Therefore, we have developed a framework that uses data parallelism to accelerate the training of 
physics informed neural networks significantly. To implement data parallelism, we use the <a href="https://github.com/horovod/horovod">Horovod</a> framework, which provides near-ideal speedup on multi-GPU regimes.

The framework currently implements a variety of recent models for forward and inverse problems in natural sciences such as
* 1d Maxwell's equation
* 1d, 2d Schrödinger's equation
* 1d, 2d Heat equation
* 1d, 3d Wave equation

## Team
- Jeyhun Rustamov
- Maksim Zhdanov
- Karan Shah (external, CASUS)


## Publications
- Stiller P., Makdani V., Pöschel F. , Richard P., Debus A., Bussmann M., Hoffmann N. (2022). Continual learning autoencoder training for a particle-in-cell simulation via streaming. Machine Learning and the Physical Sciences workshop @ NeurIPS 2022. [paper](https://arxiv.org/pdf/2211.04770)

- Shah K., Stiller P., Hoffmann N., Cangi A. (2022) Physics-Informed Neural Networks as Solvers for the Time-Dependent Schrödinger Equation. Machine Learning and the Physical Sciences @ NeurIPS 2022. [paper](https://ml4physicalsciences.github.io/2022/files/NeurIPS_ML4PS_2022_142.pdf)

- Stiller, P., Bethke, F., Böhme, M., Pausch, R., Torge, S., Debus, A., Hoffmann, N. (2020). Large-scale Neural Solvers for Partial Differential Equations. SMC 2020: Driving Scientific and Engineering Discoveries Through the Convergence of HPC, Big Data and AI, CCIS. 1315, 20-34. [paper](https://doi.org/10.1007/978-3-030-63393-6)