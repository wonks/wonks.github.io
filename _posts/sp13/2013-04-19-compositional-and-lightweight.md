--- 
layout:  post 
title:   "Compositional and Lightweight Dependent Type Inference for ML"
authors: "Suresh Jagannathan" 
date:    2013-04-19 04:15:00 
categories: Jagannathan Spring2013
--- 
## Abstract

Proving interesting and expressive safety properties of first-order programs
typically involves generating verification conditions that can be solved by a
first-order decision procedure. Higher-order functions make it complicated,
however, to infer the necessary path constraints required to do the same for
functional programs.  In this talk, we consider a solution to this problem that
encodes higher-order features into pure first-order logic formula, whose
solution can be extracted using a lightweight counterexample guided refinement
loop.  Our approach extracts initial verification conditions from dependent
typing rules derived by a syntactic scan of the program.  Specification of
higher-order functions are captured via subtyping chains generated from these
types by treating such functions as uninterpreted first-order constructs.

Our technique enables inference and compositional verification of useful safety
properties for ML programs, additionally provides counterexamples that serve as
witnesses of unsound assertions, does not entail a complex translation or
encoding of the original source program into a first-order representation, and
is fully integrated within the MLton compiler toolchain.

This is joint work with He Zhu.

