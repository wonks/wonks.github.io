--- 
layout:  post 
title:   "The Abstract Art of Modules"
authors: "Zach Sparks" 
date:    2012-02-03 04:15:00 
categories: Sparks Spring2012
--- 
## Abstract

Most widely-used programming languages have some mechanism that allows
programmers to write modular code. Haskell's typeclass system in
particular seems quite popular, as it allows programmers to take
advantage of abstract types with low syntactic overhead.

In this talk, I will give a brief introduction to ML-style module
systems, specifically using the one implemented in the SML/NJ
compiler. Starting from "representation-independent" dynamically typed
code, I will show how to use the module system to achieve true
representation independence. The main tools needed to do this are
abstract types, submodules, and functors; if there is time, I may also
demonstrate some of the more advanced features of the module system.

