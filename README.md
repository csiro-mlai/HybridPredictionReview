# LearningPDEs

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

### Generalisation

We would like to learn solutions that 

## Tools

### Dropout

Dropout gives me a kinda-sorta posterior predictive density for a given NN model.
How does this propagate through timesteps in a forward-PDE model?

### Inverse dropout

i.e. dropout for inverse problems such as learning latent fields or parameters. So if dropout gives us a posterior predictive. What if we want a posterior density over parameters, does it still work? The learned network parameters are still point estimates.

### PINN

Physics-informed neural nets, an ”implicit” representation method, give us

### Generic operator learning
