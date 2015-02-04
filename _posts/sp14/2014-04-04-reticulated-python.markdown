--- 
layout:  post 
title:   "Reticulated Python: Gradual Typing for Python"
authors: "Michael Vitousek" 
date:    2014-04-04 04:15:00 
categories: Vitousek Spring2014
--- 
## Abstract

Combining static and dynamic typing within the same language, i.e. gradual
typing, offers clear benefits to programmers. However, many open questions
remain regarding the semantics of gradually typed languages, pecially concerning
the integration of gradual typing with existing languages. I will discuss
Reticulated Python, our lightweight system for experimenting with gradual-typed
dialects of Python. Using Reticulated Python, we evaluated a gradual type system
that features structurally-typed objects and type inference for local variables.
I will discuss two dynamic semantics for casts which we implemented and
evaluated in Reticulated Python: one based on proxies and one design that
instead uses statically-inserted, use-site checks.

