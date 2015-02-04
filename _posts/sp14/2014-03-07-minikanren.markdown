--- 
layout:  post 
title:   "Recovering and enhancing miniKanren"
authors: "Jason Hemann" 
date:    2014-03-07 04:15:00 
categories: Hemann Spring2014
--- 
## Abstract

miniKanren is a relational programming language designed with purity and
portability in mind. Recently, we developed a small language kernel,
microKanren, which is somewhat low-level but powerful enough to perform actual
relational-programming tasks. We demonstrate here a miniKanren implementation
with microKanren as its core, provide some rough performance comparisons, and
describe a new implementation of unify. 

