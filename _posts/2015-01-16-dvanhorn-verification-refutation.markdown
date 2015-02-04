--- 
layout:  post 
title:   "Verification and Refutation of Behavioral Contracts with Higher-Order Symbolic Execution"
authors: "David Van Horn" 
date:    2015-01-16 04:15:00 
categories: Contracts VanHorn Spring2015
--- 
## Abstract

Behavioral software contracts are a widely used mechanism for
governing the flow of values between components. However, run-time
monitoring and enforcement of contracts imposes significant overhead
and delays discovery of faulty components to run-time.

In this talk, I will present our work on soft contract verification,
which overcomes the above issues by proving contract correctness or
producing a counterexample.

The approach is able to analyze first-class contracts, recursive data
structures, unknown functions, and control-flow-sensitive refinements
of values, which are all idiomatic in dynamic languages. It makes
effective use of an off-the-shelf solver to decide problems without
heavy encodings.  Our theoretical results include soundness and
relative completeness.  The approach is competitive with a wide range
of existing tools---including type systems, flow analyzers, and model
checkers---on their own benchmarks.

Joint work with Phuc C. Nguyen (UMD) and Sam Tobin-Hochstadt (IU)


