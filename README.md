# LearningPDEs

Various research directions in learning (S)PDEs

For now, this is a scratch pad to think through some connections, ideas and shortcomings of current approaches.

I'm writing this in markdown, but we could totally do it in LaTeX or RMarkdown if people are into that.

## Dropout

Dropout gives me a kinda-sorta posterior predictive density for a given NN model.
How does this propagate through timesteps in a forward-PDE model?

### Inverse dropout

But dropout gives us at best a posterior predictive. What if we want a posterior density over parameters, does it still work? The learned network parameters are still point estimates.

## PINN

Physics-informed neural nets, an ”implicit” representation method, give us
