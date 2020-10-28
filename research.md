---
layout: page
title: Research
---

Here are some of the research areas that I have worked in, am currently working in, or look forward to working in (in no particular order).

-----

### Information Theoretic Approaches to Quantifying Specific Causal Influence

To set the stage, consider this: does the lottery have a causal effect on an individual's spending habits? It's reasonable to expect that those who have won the lottery will answer yes and those who have not won the lottery will answer no. What happens when we use information theory to try and quantify this? Letting $$X$$ be a binary variable representing win/loss of lottery and $$Y$$ represent an individuals spending, we know that the mutual information satisfies $$I(X;Y)\le H(X) \approx 0$$, because there is virtually no chance of winning the lottery. This stands in stark contrast to something like the *average causal effect* which looks at the difference in expected difference in spending between someone who has won the lottery and someone who has not (this is big!). 

In this line of work, I look at (1) how we can use information theory to measure these kinds of effects, which I call specific causal effects, (2) what is the interpretation of these measures as compared with things like the average causal effect, and (3) how can we estimate these measures to learn more about what's going on in real datasets.

*Relevant Publications:*
- G Schamberg, W Chapman, S-P Xie, and TP Coleman, "Direct and Indirect Effects -- An Information Theoretic Perspective," *Entropy*, Volume 22, Issue 8, July 2020.
[[Entropy]](https://www.mdpi.com/1099-4300/22/8/854)
[[arXiv]](https://arxiv.org/abs/1912.10508)
[[Code Ocean]](https://doi.org/10.24433/CO.5484914.v1)
- G Schamberg and TP Coleman, "Measuring Sample Path Causal Influences with Relative Entropy," *IEEE Transactions on Information Theory*, Volume 66, Issue 5, May 2020.
[[arXiv]](https://arxiv.org/abs/1810.05250)[[IEEE Xplore]](https://ieeexplore.ieee.org/document/8856271)[[Code Ocean]](https://codeocean.com/capsule/8353473/tree/v1)
- G Schamberg and TP Coleman, "Quantifying Context-Dependent Causal Influences," *NeurIPS Workshop On Causal Learning*, December 2018. [[workshop]](https://sites.google.com/view/nips2018causallearning/home) [[pdf]]({{ site.url }}/assets/papers/2018neurips.pdf)
- G Schamberg and TP Coleman, "A Sample Path Measure of Causal Influence," *IEEE International Symposium on Information Theory (ISIT)*, June 2018.
[[IEEE Xplore]](https://ieeexplore.ieee.org/document/8437627/)
[[arXiv]](https://arxiv.org/abs/1805.03333)

-----

### Applications of Information Decompositions

The partial information decomposition (PID) problem attempts to decompose information two variables (say, $$X$$ and $$Y$$) have about a third variable ($$M$$) into four distinct components: information about $$M$$ that is uniquely encoded in $$X$$, uniquely encoded in $$Y$$, redundantly encoded in $$X$$ and $$Y$$, and synergistically encoded in $$X$$ and $$Y$$. While candidate definitions of PIDs abound, there has been less effort to apply PIDs to real-world data and justify specific PIDs in different applied contexts. Stay tuned!

-----

### Automated Anesthetic Delivery

Consider the autopilot function in airplanes. For much of the flight, we can rely on the airplane to relieve some of the burden from pilots, all the while knowing that the pilot is available to take over should it be necessary. The goal of this project is not to replace anesthesiologists, but to provide support so that at any time, the anesthesiologist can focus on the most pressing aspect of a given case. Automating the delivery of anesthetic drug requires (1) reliably characterizing a patient's anesthetic state from measured signals and (2) reliably determining the amount of drug that is needed in order to place a patient in a desired anesthetic state. My work on this problem involves building state-space models to address (1) and using reinforcement learning to address (2).

*Relevant Publications:*
- G Schamberg<sup>\*</sup>, MA Badgeley<sup>\*</sup>, EN Brown, "Controlling Level of Unconsciousness by Titrating Propofol with Deep Reinforcement Learning," *International Conference on Artifical Intelligence in Medicine (AIME)*, August 2020 (*Best Paper Award*).
- G Schamberg<sup>\*</sup>, S Chakravarty<sup>\*</sup>, T Baum, EN Brown, "Inferring neural dynamics during burst-suppression using a neurophysiology-inspired switching state-space model,” *IEEE Asilomar Conference on Signals, Systems, and Computers*, November 2020 (To appear).

<sub>* = equal contribution</sub>


-----
### Non-Markov Latent Time-Series Estimation with Non-Linear Observations

<!--![Non-Linear/Non-Markov Problems](https://raw.githubusercontent.com/gabeschamberg/gabeschamberg.github.io/master/imgs/nonmarkov_nonlin_sig.png)-->

The problem considered here is a generalization of the Kalman smoothing problem with non-Markov priors on the signal dynamics and/or the measurements obey an arbitrary log-concave likelihood model. For example, a group-sparsity prior on the dynamics could be used to promote estimates where only a few elements of the latent signal vary, or Bernoulli likelihoods could be used to model binary observations. We show that the alternating direction method of multipliers enables an iterative solution wherein the observations and dynamics can be optimized for separately and subsequently merged using a standard Kalman smoother.

*Relevant Publications:*
- G Schamberg, D Ba, and TP Coleman, “A Modularized Efficient Framework for
Non-Markov Time Series Estimation,” *IEEE Transactions on Signal Processing*, Volume 66, Issue 12, June 2018.
[[IEEE Xplore]](https://ieeexplore.ieee.org/document/8259364/)
[[arXiv]](https://arxiv.org/abs/1706.04685)
[[Code Ocean]](https://codeocean.com/2018/01/16/a-modularized-efficient-framework-for-non-markov-time-series-estimation/)
- A Allegra, A Gharibans, G Schamberg, D Kunkel, and TP Coleman, “Bayesian Inverse Methods for Spatiotemporal Characterization of Gastric Electrical Activity from Cutaneous Multi-Electrode Recording,” *PLOS ONE*, Volume 14, Issue 10, October 2019. [[pdf]](https://journals.plos.org/plosone/article/file?id=10.1371/journal.pone.0220315&type=printable)
- G Schamberg, M Wagner, D Ba, and TP Coleman, “Efficient Low-Rank Spectrotemporal Decomposition using ADMM,” *IEEE Statistical Signal Processing Workshop*, June 2016.
[[IEEE Xplore]](http://ieeexplore.ieee.org/document/7551797/)

-----