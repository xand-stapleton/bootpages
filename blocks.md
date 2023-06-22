---
layout: page
title: "Pregenerated Conformal Blocks"
---

***From the BootSTOP readme***

The pregenerated conformal blocks are computed using Mathematica in tandem with QMUL's Apocrita high performance
compute cluster. Here we describe how the spin 0 blocks were generated using the file 
*pregenerate_blocks/genblocks_6d_spin0.m*. Higher spins follow the same procedure 
with a suitable change of `spin` variable. 

First the choice of the sampling of the z-plane was made with the real and imaginary parts stored in the variables
`zre` and `zim`. Next a lower bound for the conformal weight is set within `floor`, we have consistently used 0.2 below 
the long multiplet unitarity bound so that the BootSTOP code can explore around that bound. Finally, the discretisation
of the conformal weights is set with `step` (we used 0.0005). The Mathematica code then loops evaluating the expression $$z \bar{z} a_{\Delta, \ell=0}^{\rm{at}} (z, \bar{z}) - (1-z)(1-\bar{z}) a_{\Delta, \ell=0}^{\rm{at}} (1-z, 1-\bar{z}),$$ where $a_{\Delta, \ell}^{\rm{at}}$ is defined in equation (4.5) of [arXiv:1507.05637](https://arxiv.org/pdf/1507.05637.pdf),
for all values of $z, \bar{z}$ in the z-sample with $\Delta$ starting at `floor` and increasing by `step` with 
each pass of the loop until it reaches `ceiling`. Once the loop is completed the output is exported to a csv file.
In practice setting `ceiling = floor - step + 1` with `step = 0.0005` allows the loop to complete in a reason amount
of time (~75mins) and a wide range for $\Delta$ (up to `floor + 30 - step`) can be built up by running in parallel on a 
cluster. The final, large, csv file *6d_blocks_spin0.csv* is formed by running the script 
*pregenerate_blocks/aggregate_block_data.py* with approriate values set for the variables.


## Download links:

### Non-convolved (non-Supersymmetric)
_Lattice spacing 0.0001_
- [1D]()
- [2D]()
- [4D]()
- [6D]()


### Convolved (Supersymmetric)
_Lattice spacing 0.0001_
- [1D]()
- [2D]()
- [4D]()
- [6D]()
