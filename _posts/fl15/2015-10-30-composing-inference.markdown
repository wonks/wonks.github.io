--- 
layout:  post 
title:   "Composing Inference Algorithms"
authors: "Rob Zinkov" 
date:    2015-10-30 04:15:00 
categories: Zinkov Probabilistic Fall2015
--- 
## Abstract

Probabilistic programs while, allowing many models to be easily expressed are
notorious difficult to write inference algorithms for them. Worse still, it is
difficult to extend existing a Probabilistic Programming System with a new
inference algorithm. In this talk, I will show inference algorithms can be
expressed as program transformations from probabilistic programs to
probabilistic programs. This enables defining inference procedures in a more
modular  and simpler way. The resulting programs, after these transformations,
have a running time comparable to that of a hand-written inference procedure.

