--- 
layout:  post 
title:   "Modeling Application Memory Behavior at a High Level"
authors: "Arun Chauhan" 
date:    2011-02-04 04:15:00 
categories: Chauhan Spring2011
--- 
## Abstract

The problem of modeling memory locality of applications to guide 
compiler optimizations in a systematic manner is an important unsolved 
problem, made even more significant with the advent of multi-core and 
many-core architectures. In the first part of the talk I will describe an 
approach based on a novel source-level metric, called static reuse 
distance, to model the memory behavior of applications written in MATLAB. 
We use MATLAB as a representative language that lets end-users express 
their algorithms precisely, but at a relatively high level. MATLAB's 
"high-level" characteristics allow the static analysis to focus on large 
objects, such as arrays, without losing accuracy due to processor-specific 
layout of scalar values in memory.

In the second part of the talk I will describe a model to predict the 
performance of MATLAB programs on GPUs and use it for automatic 
partitioning of MATLAB programs across CPUs and GPUs, in order to maximize 
parallelism.  We use a heuristic algorithm to solve the hard partitioning 
problem and show experimental results to demonstrate its effectiveness.

Finally, I will outline some ideas that bring the problems of locality and 
parallelization together.

