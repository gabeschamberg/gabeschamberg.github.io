---
layout: post
title: Neural Networks and Logistic Regression
---

### Introduction

If you are reading this post, you have likely heard neural networks referred to as "black boxes". While it may take us quite some time to be comfortable totally rejecting this description of neural networks, this "black box" label leaves the impression that there is little to be understood about the inner workings of neural networks, which is simply not the case. There are numerous resources that address some of the natural questions that arise when dealing with neural networks. One of the finest examples is [Colah's Blog](http://colah.github.io/). [One interesting post](http://colah.github.io/posts/2014-03-NN-Manifolds-Topology/) relates the topology of the dataset to the required number of hidden units. [A second post](http://colah.github.io/posts/2014-07-NLP-RNNs-Representations/) discusses how NLP models learn relationships between words that are familiar to us as humans (such as boy is to girl as his is to hers) as a means of understanding natural language. In other words, in order to accomplish an arbitrary language task, neural networks may learn to think about language in a way that is similar to how humans do.

While both of these posts aid in illuminating the inner workings of neural networks, they are concerned with wholly different questions. While the first post contains visualizations of small scale neural nets learning to classify low-dimensional datasets, the second post attempts to identify how a deep neural network makes sense of the massive language datasets. It seems to me that this gap is largely responsible for the feeling that neural networks are black boxes -- on the one hand we can begin to understand how neural networks learn through small examples, but for the applications that are really of interest, we are left trying to identify aspects of the trained networks that are interpretable without truly understanding the function of every aspect of the model.

What's the point? Neural networks are complicated, and this post is certainly not going to do much (if anything) to demystify the "black box", but hopefully it can help you to chip away at the problem from the "understanding how neural networks learn through small examples" end of spectrum. In fact, I will be moving all the way to the very edge of the spectrum, as my goal here is to relate neural networks to perhaps the simplest tool for binary classification problems, *logistic regression*. As shown by this [Google search](http://www.google.com/search?q=neural+network+logistic+regression), the observation of a connection between logistic regression and neural networks is not a novel one. Nevertheless, I find it a useful observation for stepping through basic examples and trying to learn what exactly is going on.

I will include some code snippets throughout the post to illustrate key points, but because this is not a coding lesson, most of the code generated will be omitted. If you'd like to see how all the figures were generated and play around with the code, you can download this [iPython notebook]({{ site.url }}/assets/posts/2017-08-10-neural-networks-and-logistic-regression/neural_nets_logistic_regression.ipynb). Now, let's get started!

### Logistic Regression

Let's start by getting an intuitive understanding of logistic regression. Suppose we have two classes of data existing in 2-dimensional space. The orange class is a cluster centered at the point $$ (X_1,X_2) = (0,0)$$, and the blue class is a cluster centered at $$(X_1,X_2) = (5,5)$$. Now suppose we have $$500$$ points from each class, and using these points, want to learn how to tell whether a new point belongs to the orange or blue class.

![logreg1.png]({{ site.url }}/assets/posts/2017-08-10-neural-networks-and-logistic-regression/logreg1.png)

It is pretty clear here that the pink point belongs to the blue class. How can we formalize this seemingly obvious observation?






### Parting Thoughts

While there are some [amazing](http://http://playground.tensorflow.org/) [resources](http://cs.stanford.edu/people/karpathy/convnetjs/) for experimenting with neural networks, I often find myself fiddling with parameters and convincing myself I get how it works when that is not actually the case. I

```python
def function():
    print("hello")
```