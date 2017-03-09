---
layout: page
title: Research
---

### Time-Varying Causal Inference

![Time-Varying Causality](https://raw.githubusercontent.com/gabeschamberg/gabeschamberg.github.io/master/imgs/causality.png)

We consider the questions:

1. Do two observed time series have a causal influence on one another?
2. How do these influences change over time?

Using a [Granger causality](http://www.scholarpedia.org/article/Granger_causality) viewpoint, at every time *t*, the causal influence from *X* to *Y* is meant to represent how much better we can predict *Y* given its past *and* the past of *X* than if we were given the past of *Y* alone. To actually acquire these measures, we leverage tools in [sequential prediction](https://www.eng.tau.ac.il/~meir/articles/32%20Universal%20Prediction.pdf) and [directed information](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.36.5688&rep=rep1&type=pdf).

-----

### Non-Linear / Non-Markov Latent Time-Series Estimation

![Non-Linear/Non-Markov Problems](https://raw.githubusercontent.com/gabeschamberg/gabeschamberg.github.io/master/imgs/nonmarkov_nonlin_sig.png)

We consider the problem of estimating a latent multi-dimensional time-series given noisy measurements and knowledge of the dynamics of the signal. In the case of a Markov signal with linear dynamics and Gaussian measurements, the problem can be solved using the [Kalman filter](https://en.wikipedia.org/wiki/Kalman_filter).

We consider the class of problems where the underlying signal is non-Markov and/or the measurements obey and arbitrary log-concave likelihood model. We propose a framework that uses the [Alternating Direction Method of Multipliers](http://stanford.edu/~boyd/admm.html) to decompose problems of this nature into smaller, easy to solve subproblems.

An application of this method to acquire low-rank spectrotemporal decompositions was published at the IEEE Workshop on Statistical Signal Processing in 2016 and can be found [here](http://ieeexplore.ieee.org/document/7551797/).

-----