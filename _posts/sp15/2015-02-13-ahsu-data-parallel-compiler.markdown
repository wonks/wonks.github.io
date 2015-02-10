--- 
layout:  post 
title:   "The Key to a Data Parallel Compiler" 
authors: "Aaron Hsu" 
date:    2015-02-13 04:15:00 
categories: Hsu Spring2015
--- 
## Abstract

How do you write a data parallel compiler? What does that even mean? In this
demonstration I’ll show how I’ve constructed the Co-dfns compiler, which is
written using a data flow, branchless style that shifts control logic from the
program text to the data representation, in contrast to traditional compiler
constructions which rely heavily on conditional branching and dispatch. The Key
operator turns out to underly the most significant compiler passes, enabling a
concise expression of many compiler passes. I will demonstrate how I combine the
Key operator together with an encoding of parent-child relationships to permit
computing over sub-trees defined by parent-child constraints.

*This is early work presented in an interactive context, intended to present a well practiced idea (compilers) in a fresh manner, hopefully to everyone’s enjoyment.* 

