--- 
layout:  post 
title:   "A Combinator Library for MCMC Sampling"
authors: "Praveen Narayanan" 
date:    2014-11-21 04:15:00 
categories: Narayanan Fall2014
--- 
## Abstract

In this talk I will present an initial version of a Haskell library designed to
ease the construction and use of MCMC samplers. I will first introduce the MCMC
method and motivate its application on a concrete example - the Gaussian Mixture
Model (GMM). I will then describe an MCMC sampler for a GMM, and show how this
sampler can be made more modular by using combinators from the library. The goal
is to convince the audience of the benefits of applying paradigms such as higher
order functions and lazy evaluation to the domain of MCMC sampling. No prior
experience with MCMC samplers is required, and questions are strongly
encouraged.
