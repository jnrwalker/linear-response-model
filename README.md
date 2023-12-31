# linear-response-model

This notebook is an exploratory investigation of the linear response model. The linear response model can be mathematically expressed as:

$$ x=𝜂_t (x_{t-1}+𝜆(x_{s}-x_{t-1})) $$

According to the model, the state of an ecosystem at a particular time, depends on the state of the system at the previous time point, as well as the rate at which the prior state deviates from the steady state, which is simply the fixed point. In this model, a multiplicative white noise term is multiplied to represent the global stochastic changes, known as crackling noise, or Barkhausen noise. Crackling noise has been generalized to model global stochastic changes in various complex choatic systems, from earthquakes to financial markets and ecosystems. The noise term is sampled from a normal Gaussian distribution with unit mean and 0.01 standard deviation.

In particular, we investigate how varying eigenvalues changes the behaviour of this model close to a tipping point (where taking the limit of the eigenvalue approaching zero). We show that close to a tipping point or at the marginally stable condition, the variance and hence standard deviations increase exponentially. Furthermore we show that the linear response model exhbitis a lag-1 autocorrelation approaching 1 (in other words total autocorrelation) as the eigenvalue approaches zero.
