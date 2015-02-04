--- 
layout:  post 
title:   "Combining Denotational and Operational Semantics for Scalable Proof Development"
authors: "Adam Foltzer" 
date:    2011-09-23 04:15:00 
categories: Foltzer Fall2011
--- 
## Abstract

Interpreters offer a convenient and intuitive way for programmers to reason
about language behavior through denotational semantics. However in a setting
like Coq, where all recursive functions must provably terminate, it is
impossible to write interpreters for non-terminating languages. The standard
alternative is to inductively define operational semantics, but this can yield
proofs that are difficult to automate, particularly in the presence of changing
language features.

This talk presents a combined approach, where an interpreter is used in
combination with operational semantics to prove type preservation of a small
functional language. To demonstrate the scalability of the Coq development, let
expressions and pair types will be added and preservation will be proved again
with only one extra line of proof script.

This technique and development are adapted with permission from Greg Morrisett's
lectures at the 2011 Oregon Programming Languages Summer School, and are
available at his web site (http://www.eecs.harvard.edu/~greg/oplss/).

Although this talk is presented in Coq, I will briefly introduce the basic
syntax as we encounter it, which should be accessible to anyone with experience
in a typed functional language like ML, Scala, or particularly Haskell with
GADTs.

