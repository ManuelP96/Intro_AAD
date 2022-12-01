# Introduction to Algorithmic Adjoint Differentiation

In recent years, the computational cost of some mathematical operations in finance has increased every day due to the complexity of financial products or the models behind their valuation. In addition, the classical techniques (that is, finite differences) do not give us exact values of the derivatives but approximations of them.

For that reason, when reading about Adjoint Differentiation and its application to finance (mainly from Savine's work), we are interested in its previous results in terms of reducing the time and computational cost of calculating sensitivities.

The first objective was to understand the mathematics behind this technique and a first application (Dupire's Volatility Model), this objective was developed within a study group at the Faculty of Economics of the Universidad del Rosario during the second semester of 2022. Therefore, this repository contains the material (Videos and Slides of the sessions) used and produced at that time.

### [Session 1](https://youtu.be/0DpfCDToc4Q)

After a brief exposition of mathematical concepts, we introduce the term *adjoint* and its formula. Then we give a simple calculus example of the adjoints and its relation with the partial derivatives of a function.

### [Session 2](https://youtu.be/vdR9eZ8OZ9A)

We translate the calculus-type definitions of AAD into matrix-type definitions for Forward and Adjoint modes to understand how algorithms should be developed, and give the example of computing partial derivatives for a simple function, with [Forward Mode](https://colab.research.google.com/drive/1bRna7-7YnNduzqLAAPJ4D4QVJMpG7u0F?usp=sharing) and [Adjoint Mode](https://colab.research.google.com/drive/113uQx2w5kIJwiIp_RHz2LGXftUsMc_f_?usp=sharing).

### [Session 3](https://youtu.be/ZiHsWkEyYyg)

We implemented, as a first simple example in Finance, the AAD technique for computing greeks in the Black-Scholes-Merton Model for a European Call Option. The implementation in [Python](https://colab.research.google.com/drive/1LFKCGPuzqfQbc70qQi22CczFlQ_It2kC?usp=sharing) is not optimized and just follows the matrix-type algortihm.

### [Session 4](https://youtu.be/dIn7LU7E09A)

Now, we review the paper *[Differential Machine Learning](https://arxiv.org/pdf/2005.02347.pdf)* while exploring the possible research using AAD, here the main idea is that AAD is equivalent to Backpropagation in the Machine Learning language, so Savine & Huge combined Forward and Adjoint Mode into a *Twin Network*. Here we understand that Tensorflow2 is a Python library written in C++ which has already implemented AAD in the GradientTape API.

### [Session 5](https://youtu.be/RSYn_m4zpxs)

We explain the Dupire's Volatility Formula and review the Savine's implementation on C++ of this model.

### [Session 6](https://youtu.be/f4k0BozqJ4I)

We implement the Dupire's Model example in [Python](https://colab.research.google.com/drive/1b-wMIzUPO9-KUHtiXKn1xdFvdGiuT2Hw?usp=sharing) which are useful to understand how AAD reduces time and computational cost using the record of calculations in a *Tape*.
