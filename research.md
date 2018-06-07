---
layout: page
title: Research
---

### Time-Varying Causal Inference

![Time-Varying Causality](https://raw.githubusercontent.com/gabeschamberg/gabeschamberg.github.io/master/imgs/causality3.png)

How can we tell when one time series is having a *causal* effect on another time series? How can we assess the changes that occur in this causal relationship over time?

We adopt a [Granger causality](http://www.scholarpedia.org/article/Granger_causality) viewpoint, where at every time $$t$$, the causal influence from $$X$$ to $$ Y $$ is represents how much better we can predict $$ Y $$ given its past *and* the past of $$ X $$ than if we were given the past of $$Y$$ alone. We note that this relationship may change depending on the *actual values* that these time series take on, as opposed to being solely dependent on the model, as with [directed information](https://arxiv.org/pdf/1201.2334.pdf) and [transfer entropy](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.85.461). As such, we are researching a novel measure of causality that takes on different values for different process realizations, even in stationary processes. To actually acquire these measures, we leverage tools in [sequential prediction](https://www.eng.tau.ac.il/~meir/articles/32%20Universal%20Prediction.pdf).

*Relevant Publications:*
- "A Sample Path Measure of Causal Influence", *IEEE International Symposium on Information Theory (ISIT)*, June 2018, To Appear.
[[arXiv]](https://arxiv.org/abs/1805.03333)

-----

### Non-Linear / Non-Markov Latent Time-Series Estimation

![Non-Linear/Non-Markov Problems](https://raw.githubusercontent.com/gabeschamberg/gabeschamberg.github.io/master/imgs/nonmarkov_nonlin_sig.png)

We consider the problem of estimating a latent multi-dimensional time-series given noisy measurements and knowledge of the dynamics of the signal. In the case of a Markov signal with linear dynamics and Gaussian measurements, the problem can be solved using the [Kalman filter](https://en.wikipedia.org/wiki/Kalman_filter).

We consider the class of problems where the underlying signal is non-Markov and/or the measurements obey and arbitrary log-concave likelihood model. We propose a framework that uses the [Alternating Direction Method of Multipliers](http://stanford.edu/~boyd/admm.html) to decompose problems of this nature into smaller, easy to solve subproblems.

*Relevant Publications:*
- “A Modularized Efficient Framework for
Non-Markov Time Series Estimation”, *IEEE Transactions on Signal Processing*, Volume 66, Issue 12, June 2018.
[[IEEE Xplore]](https://ieeexplore.ieee.org/document/8259364/)
[[arXiv]](https://arxiv.org/abs/1706.04685)
[[Code Ocean]](https://codeocean.com/2018/01/16/a-modularized-efficient-framework-for-non-markov-time-series-estimation/)
- “Efficient Low-Rank Spectrotemporal Decomposition using ADMM”, *IEEE Statistical Signal Processing Workshop*, June 2016.
[[IEEE Xplore]](http://ieeexplore.ieee.org/document/7551797/)

-----