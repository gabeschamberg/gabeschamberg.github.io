---
layout: post
title: Three Questions in Causal Influence
---

### Introduction

For the past year or so, my research efforts have been primarily focused on questions in causal inference. While I have thoroughly enjoyed studying this area, approaching causality from an electrical engineering perspective has its difficulties. In particular, I find it challenging to establish a balance between philosophy and theory. To be clear, when I say "philosphy", I am referring to non-mathematical justifications for my work. I worry that if I lean too heavily on the non-mathematical component of my work then I'll appear to be making a stronger statement about the fundamental nature of causality than I intend to. On the other hand, if I rely solely on the math to do the talking, then it becomes pretty difficult to tell a compelling story.

I've come to believe that the balance is best achieved by establishing context. As a first step, I'm certainly willing to accept that I don't know what causality truly is (or whether it exists for that matter). If we're all comfortable with that, then we are free to set the stage. We can consider whatever questions in causality we like, come up with mathematical tools for answering those questions, and discuss whether or not those tools make sense intuitively. I have come to believe that this exercise is not only important for ensuring that my research is well received, but that it is important if I hope for my methods to be used elsewhere. After all, the purpose of developing methods for causal inference is for them to be used to answer interesting questions. Unfortunately, if one is not very clear about what kind of questions their method is designed to answer, then it may be used on the wrong questions and, as a result, get the wrong answers.

Ultimately, the above rambling is a disclaimer. I want to be very clear that I am not claiming that the following perspective on causality is the **right** perspective. It's **a** perspective, and hopefully one that you will find interesting.

## Some Notation

Suppose we have two discrete random sequences, $$X_1,X_2,\dots,X_n$$ and $$Y_1, Y_2,\dots, Y_n$$. A superscript will denote a collection of samples as $$X^i=(X_1,\dots,X_i)$$. Let $$P$$ denote a probability mass function (pmf), and suppose we know the full joint distribution over both sequences $$P(X^n,Y^n)$$. If we assume that there is no instantaneous causation, then we will be interested in the following factorization of the joint distribution using the chain rule:

$$
\prod_{i=1}^n P(X_i \mid X^{i-1},Y^{i-1})P(Y_i \mid X^{i-1},Y^{i-1})
$$

Next, let lowercase letters represent realizations of a random entity. For example, we will say that the probability that $$X_i$$ takes on a value $$x_i$$ is $$P(x_i)$$. This should be enough to get us going, so let's dive in.

## __Question 1__ - Does $$Y^{i-1}$$ Cause $$X_i$$?

Before getting into the math, let's consider some examples:

- Does dieting impact weight loss?
- Does the New York Stock Exchange (NYSE) influence the Shanghai Stock Exchange (SSE)?
- Does the climate affect extreme weather events?

My avoidance of the word "cause" in these questions is intentional.