---
title: 'Continual learning autoencoder training for a particle-in-cell simulation via streaming'
collection: publications
permalink: /publication/2022-11-09-patrick-streamingML
excerpt: 'Continual learning autoencoder training for a particle-in-cell simulation via streaming'
date: 2022-11-09
venue: 'Machine Learning and the Physical Sciences @ NeurIPS 2022'
paperurl: 'https://arxiv.org/abs/2211.04770'
citation: 'Stiller P., Makdani V., Pöschel F. , Richard P., Debus A., Bussmann M., Hoffmann N. (2022). Continual learning autoencoder training for a particle-in-cell simulation via streaming. Machine Learning and the Physical Sciences workshop @ NeurIPS 2022.'
---

The upcoming exascale era will provide a new generation of physics simulations. These simulations will have a high spatiotemporal resolution, which will impact the training of machine learning models since storing a high amount of simulation data on disk is nearly impossible. Therefore, we need to rethink the training of machine learning models for simulations for the upcoming exascale era. This work presents an approach that trains a neural network concurrently to a running simulation without storing data on a disk. The training pipeline accesses the training data by in-memory streaming. Furthermore, we apply methods from the domain of continual learning to enhance the generalization of the model. We tested our pipeline on the training of a 3d autoencoder trained concurrently to laser wakefield acceleration particle-in-cell simulation. Furthermore, we experimented with various continual learning methods and their effect on the generalization.
[Download paper here](https://arxiv.org/abs/2211.04770)

Recommended citation: Stiller P., Makdani V., Pöschel F. , Richard P., Debus A., Bussmann M., Hoffmann N. (2022). Continual learning autoencoder training for a particle-in-cell simulation via streaming. Machine Learning and the Physical Sciences workshop @ NeurIPS 2022.
