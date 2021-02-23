---
nocite:
- '@*'
bibliography: refs.bib
link-citations: true
title: Learning PDEs
---

# Learning PDEs

Various research directions in learning approximations to (S)PDEs

For now, this is a scratch pad to think through some connections, ideas and shortcomings of current approaches.

I'm writing this in markdown, but we could totally do it in LaTeX or RMarkdown if people are into that.

## Problems to solve

### Computational efficiency

PDE solvers are often slow

### Learning latent fields

### Learning parameters

### Interpolating

An obvious way to start it to learn a PDE over a grid or mesh.
This is unsatisfactory for a variety of reasons (large GPU memory requirement, scale-dependent.)
Can we move from grid coordinates to continuous space/time?

### Generalisation/conditionalisation

We would like to learn solutions that 

## Tools

### Dropout

Dropout gives me a kinda-sorta posterior predictive density for a given NN model.
How does this propagate through timesteps in a forward-PDE model?

@FoongPathologies2019; @GalConcrete2017; @GalDropout2015

### Chaos expansion

Learning a basis expansion for an approximate SDE

### PINN

Physics-informed neural nets, an ”implicit” representation method, give us rapid neural networks.
See [PINNs](https://danmackinlay.name/notebook/ml_pde.html#learning-a-pde).

### Generic operator learning

See, e.g. [Fourier neural operators](https://danmackinlay.name/notebook/ml_pde.html#fourier-neural-operator).

These seem favourable in that they learn rapid approximations to PDEs. However, it is unclear how to conduct an error analysis upon them or do general inference.

## To build this document

This markdown document renders using [pandoc](https://pandoc.org/) with the following command:

```bash
pandoc -s --citeproc README.md -o README.html
```

## References

::: {#refs}
:::
