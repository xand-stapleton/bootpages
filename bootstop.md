---
layout: page
title: "BootSTOP (Bootstrap STochastic OPtimiser)"
---
***From [BootSTOP repository README](https://github.com/vniarchos/bootstop)***

---
<!-- TOC -->
* [Contents](#bootstop-bootstrap-stochastic-optimiser)
  * [Overview](#overview)
  * [Installation](#installation)
  * [Running the code](#running-the-code)
  * [References](#references)
<!-- TOC -->

## Overview
BootSTOP is a Python package for determining CFT data (OPE-coefficients squared and scaling dimensions) 
which minimise a theory's truncated crossing equation. To do this the code can apply either a custom PyTorch 
implementation of the Soft-Actor-Critic algorithm
or one of the algorithms within the PyGMO package (information about PyGMO can be found 
[on the PyGMO website](https://esa.github.io/pygmo2/)). 

At present the crossing equation for each of the following CFTs is coded within BootSTOP: 
1D defect CFT (see [4]), 2D c=1 compactified boson CFT (see [1,2]) 
and the 6D (2,0) SCFT (see [3]). See [1-4] and the references within for comprehensive background.

## Installation
For installation instructions see [our getting started page](https://github.com/vniarchos/BootSTOP/blob/main/requirements/getting_started.md).

Then you will need to follow [download the blocks from our block page](blocks.md)
from where you should copy the pre-generated conformal block files and place
them within the relevant *block_lattices* 
folder in your local BootSTOP repository.

## Running the code

This repository contains several configured config and run files so that you can immediately start solving.
For example, executing the command:
   ```
   python3 run_pygmo_1d_deriv.py
   ```
will apply PyGMO's IPOPT algorithm to the (derivative form) crossing equation of the 1D defect CFT 
truncated to 62 operators.



## References
- [1] G. Kantor, V. Niarchos and C. Papageorgakis,
*Solving Conformal Field Theories with Artificial Intelligence*,
Phys. Rev. Lett. 128 (2022) [arXiv:2108.08859](https://arxiv.org/abs/2108.08859)
- [2] G. Kantor, V. Niarchos and C. Papageorgakis,
*Conformal bootstrap with reinforcement learning*,
Phys. Rev. D 105 (2022) [arXiv:2108.09330](https://arxiv.org/abs/2108.09330)
- [3] G. Kantor, V. Niarchos, C. Papageorgakis and P. Richmond,
*6D (2,0) bootstrap with soft-actor-critic algorithm*,
Phys. Rev. D 107 (2023) [arXiv:2209.02801](https://arxiv.org/abs/2209.02801)
- [4] V. Niarchos, C. Papageorgakis, P. Richmond, A. G. Stapleton and M. Wooley,
*Bootstrability in Line-Defect CFT with Improved Truncation Methods*, [arXiv:2306.15730](https://arxiv.org/abs/2306.15730)

