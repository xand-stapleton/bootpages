---
layout: page
title: "BootSTOP-multi-correlator (Bootstrap STochastic OPtimiser)"
---
***From [BootSTOP-multi-correlator repository README](https://github.com/jchryssanthacopoulos/BootSTOP-multi-correlator)***

---
## Overview
BootSTOP is a Python package for determining CFT data (OPE-coefficients squared
and scaling dimensions) which minimise a theory's truncated crossing equation.
This page presents BootSTOP-multi-correlator, a multi-objective implementation
of BootSTOP used to determine the CFT data of the 3D Ising model. Like
BootSTOP, BootSTOP-multi-correlator employs the algorithms within the PyGMO
package (information about PyGMO can be found [on the PyGMO website](https://esa.github.io/pygmo2/)). 


## Installation
For installation instructions see [our getting started page](https://github.com/jchryssanthacopoulos/BootSTOP-multi-correlator/blob/main/README.md).

The most efficient way to run BootSTOP-multi-objective is with its sibling
package [GoBlocks](https://github.com/xand-stapleton/goblocks), a fast,
parallel conformal block generator.


## References
- [1] J. Chryssanthacopoulos, V. Niarchos, C. Papageorgakis, A. G. Stapleton
*Efficient Conformal Block Evaluation with GoBlocks*,
[arXiv:2603.10627](https://arxiv.org/abs/2603.10627)
