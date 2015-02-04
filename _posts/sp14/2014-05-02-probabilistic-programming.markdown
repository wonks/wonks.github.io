--- 
layout:  post 
title:   "Probabilistic Programming for the PL researcher"
authors: "Rob Zinkov" 
date:    2014-05-02 04:15:00 
categories: Zinkov Spring2014
--- 
## Abstract

Bayesian inference tasks and machine learning in general we are often inferring
some latent quantity given some observed data and a theory for how this latent
quantity generated this data. The idea behind probabilistic programming
languages is that this theory of how the data was generated is best expressed as
a programming language. In this talk, I will introduce a denotational semantics
for one such language based on measures which can be understood as unnormalized
probability distributions. I will then introduce an operational semantics
based on Markov-Chain Monte Carlo (MCMC) sampling. Finally, I will show that
these two semantics are not isomorphic and mappings  between the two do not
preserve algorithmic performance. I will highlight  applications that range
from outlier detection to clustering algorithms to predicting who will run a
game of tug-of-war.

