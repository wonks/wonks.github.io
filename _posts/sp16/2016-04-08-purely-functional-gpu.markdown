--- 
layout:  post 
title:   "Purely Functional GPU Programming"
authors: "Mike Vollmer"
date:    2016-04-08 04:15:00 
categories: Vollmer Spring2016
--- 

## Abstract

GPUs are massively parallel multi-core processors optimised for workloads with a
large degree of SIMD parallelism. While they can offer excellent performance,
they generally provide a restrictive programming model and require expert
knowledge to fully utilize. 

In this talk, I'll give a general tutorial on programming in Accelerate, an
embedded domain-specific language for array programming in Haskell. I'll show
how Accelerate addresses these issues, making efficient GPU programming
accessible to ordinary functional programmers.
