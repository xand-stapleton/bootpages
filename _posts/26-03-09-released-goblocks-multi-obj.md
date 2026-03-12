---
title:  "Release of GoBlocks and BootSTOP-multi-correlator"
mathjax: true
layout: post
categories: media
---
*Authors: J. Chryssanthacopoulos, V. Niarchos, C. Papageorgakis, A.G. Stapleton*

__Paper available on the arXiv at [2603.10627](https://arxiv.org/abs/2603.10627). Included as reference [1]__

## Abstract

Conformal blocks in odd spacetime dimensions are not known in closed analytic form. To facilitate efficient computations in the conformal bootstrap, we introduce GoBlocks: a novel conformal block generator implemented in the Go programming language, designed for rapid, on-the-fly, parallel evaluation using recursive relations. The package supports both multi-point and derivative-based bootstrap approaches and allows flexible control over accuracy and performance. We benchmark GoBlocks against the scalar_blocks package, finding significant speed improvements in applications where computational speed and moderate accuracy are critical, but ultra-high precision is not essential. As an illustration, we apply GoBlocks to the mixed-correlator bootstrap of the three-dimensional Ising model, formulated as a non-convex optimisation problem in a suitable truncation scheme. We simultaneously optimise over external scaling dimensions and OPE CFT data. In addition, we discuss how the approach scales as we increase the number of mixed correlators in more general O(N) vector models.

## References
- [1] J. Chryssanthacopoulos, V. Niarchos, C. Papageorgakis, A. G. Stapleton
*Efficient Conformal Block Evaluation with GoBlocks*,
[arXiv:2603.10627 ](https://arxiv.org/abs/2603.10627)
