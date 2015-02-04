--- 
layout:  post 
title:   "A Loopy Introduction to Dependence Analysis"
authors: "Lindsey Kuper" 
date:    2011-12-09 04:15:00 
categories: Kuper Fall2011
--- 
## Abstract

A parallelizing or vectorizing compiler for a sequential programming
language must rearrange the execution order of program statements
while still preserving the meaning of a computation.  The goal of a
compiler dependence analysis is to produce a dependence graph that
captures which constraints on execution order are critical, so that
the rest of them can be loosened.  This dependence information can
then be used to direct the generation of vectorized code in a
semantics-preserving way.  In this short talk, I'll introduce a few
basic notions of the theory of data dependence, drawn mostly from the
first two chapters of "Optimizing compilers for modern machinery: a
dependence-based approach" by Allen & Kennedy
(http://dl.acm.org/citation.cfm?id=502981).  To make the ideas
concrete, JP Verkamp and I have been implementing a data dependence
analysis for a tiny toy language, which I've dubbed "Loopy".  We'll do
a quick demo of our dependence analysis, which was implemented using
syntax-rules, and if time permits (read: if I get it working in
time!), I'll show a second implementation done using the PLT Redex
semantics engineering tools.  Our work in progress is available at
https://github.iu.edu/lkuper/find-deps.
