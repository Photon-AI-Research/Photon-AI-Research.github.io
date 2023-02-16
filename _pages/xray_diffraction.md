---
permalink: /xray_diffraction/
title: "Xray Diffraction"
author_profile: true
redirect_from: 
  - /xrd/
  - /xrd.html
---

We are currently developing a one-step reconstruction method for inverting SAXS data during experiments at synchrotrons like [DESY](https://desy.de) or our [HIBEF](https://www.hzdr.de/db/Cms?pOid=50566&pNid=694) beamline at [EuropeanXFEL](https://www.xfel.eu). Due to the loss of the phase information, there is often more than one solution for each diffraction pattern. The conditional Invertible Network, a generative model, is able to reconstruct all possible solutions in a matter of milliseconds. The network is trained on perturbed simulated data only with a data-driven negative log-likelihood loss and is able to reconstruct most experimental data.

The library **nfPhasing** expands the data loss by a physics-driven loss that integrates knowledge about the underlying scattering processes.


<iframe
    width="640"
    height="480"
    src="https://www.youtube.com/watch?v=dslwFktsnmM&t=2s"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe>


The general idea is that a conditional Normalising Flow is learning a mapping from experimentally acquired diffraction pattern(s) **I** and some prior distribution to the predictive posterior distribution of electron densities **u**. The neural network is trained by a data-driven objective as well as a Physics-based loss. The former allows for very fast inference (i.e. reconstruction) on data similiar to our training data while the latter enables reconstruction of objects that are out-of-distribution to the training data.

**nfPhasing** is covering the following modalities:
- 1d/2d Small-angle X-ray scattering (at Grazing Incidence)
- 2d Ptychography
- 2d Holography / Phase Contrast Imaging

## Team
* Ritz-Ann Aguilar
* Erik Thiessenhusen
* Maksim Zhdanov
* Nicolas Schmitt

## Publications
- Achilles, S., Ehrig, S., Hoffmann, N., Kahnt, M., Becher, J., Fam, Y., Sheppard, T., Brückner, D., Schropp, A., Schroer, C. (2022). GPU-accelerated coupled ptychographic tomography. Proc. SPIE 12242, Developments in X-Ray Tomography XIV, 122420N. [paper](https://doi.org/10.1117/12.2633102)

- Zhdanov, M., Randolph, L., Kluge, T., Nakatsutsumi, M., Gutt, C., Ganeva, M., Hoffmann, N. (2022). Amortized Bayesian Inference of GISAXS Data with Normalizing Flows. Machine Learning and the Physical Sciences workshop @ NeurIPS 2022. [paper](https://arxiv.org/abs/2210.01543)

- Liu, Y., Shao, Z., Teng, Y., Hoffmann N. (2021). NAM: Normalization-based Attention Module. ImageNet PPF @ NeurIPS 2021. [paper](https://arxiv.org/abs/2111.12419)

- Liu, Y., Shao, Z., Hoffmann, N. (2021). Global Attention Mechanism: Retain Information to Enhance Channel-Spatial Interactions. arXiv:2112.05561v1. [paper](https://arxiv.org/abs/2112.05561)