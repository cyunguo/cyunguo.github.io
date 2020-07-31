---
layout:     post
title:      Probability Studying
subtitle:   Probability Theory and Examples From Rick Durrett
date:       2020-07-31
author:     YC
header-img: img/post-bg-kuaidi.jpg
catalog: true
tags:
    - Probability
---

> The ideas in blog mainly comes from the Probability: Theory and Examples --- Rick Durrett.

##### 1.  Measure space and probability.

When we construst a measureable space, we actually need the $ \sigma -field$ which is kind of "complete", the $\sigma-filed$ is actually very nature if we consider a probability space and the operations we can do on the probabilty space. 

After constructing the $\sigma-field$, we need to mapping of it on the Borel set since Borel set is something easier to deal with. The thing is we actually need the measureable function which will be the random variable in probability space. The thing is we need one-one mapping here. I used to feel a little bit confused about the inverse part, the reason is I actually did not fully understand the meaning of the Borel set. Actually for very simple system, very simple probability space, just like coin tossing, we do not need to map it to the Borel set, but at the same time our measure will not be on the Borel set neither. 

So, actually what we did is to map the original space to the Borel set which is much easier to calculate since now we can just use the numbers to represent the different events in the original space. (Notice : There can be a lot of measureable functions which are also the random variables in the probability space. )

##### 2. Conditional probability.

The conditions actually correspond to the change of the space ( $\sigma-field$ ). 

##### 3. Expectation and uncorrelated.

$\mathbf{E}[XY]=\mathbf{E}[X]\mathbf{E}[Y]$ holds when they are independent, positive and the expectation is finite. It is easy to understand the conditions considering the integration. At same time, the equation above may hold without independence requirement. In such circumstance, it refers to the uncorrelated. It also suggests that independent means uncorrelated.

Furthermore, if $\mathbf{E}[XY]=\mathbf{E}[X]\mathbf{E}[Y], var(X+Y)=var(X)+var(Y)$.

##### 4. Sum of 2 variables.

Let $X,Y$ be independent with probability density function $f(X),g(Y)$, then $Z=X+Y$ has density
$$
h(Z)=\int f(Z-Y)g(Y)dY
$$
2 Example: Gamma distribution and Gaussian distribution.

Noticed: from the convolution we actually can derive the Gamma distribution by using the sum of exponential distribution.

Normal distribution : $X\sim (\mu_1,a_1), Y\sim(\mu_2,a_2), X+Y \sim (\mu_1+\mu_2,a_1+a_2)$.

##### 5. Large number theorem.

###### 1) $L^2$ Weak Laws. 

Let $X_1,X_2,...,X_n$ be uncorrelated RV with $\mathbf{E}[X_i]=\mu$ and $var(X_i)\leq C <\infty$. Let $S_n=X_1+...+X_n$, we have $S_n/n\rightarrow \mu$ in $L^2$ and in probability.

Noticed that converage in $L^2$ actually means that variance converge to 0. The interesting part is that the normal binomial distribution can lead to polynomial approximation of a contiuous function.

