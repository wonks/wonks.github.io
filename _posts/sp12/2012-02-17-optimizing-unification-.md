--- 
layout:  post 
title:   "Optimizing Unification"
authors: "Wren Thornton" 
date:    2012-02-17 04:15:00 
categories: Thornton Spring2012
--- 

* (Slides)[http://llama.freegeek.org/~wren/pubs/unification-intro-mcmaster.pdf]
* (Slides)[http://llama.freegeek.org/~wren/pubs/unification-opt-mcmaster.pdf]
* (Implementation)[http://hackage.haskell.org/package/unification-fd]

## Abstract

Unification has many diverse applications, from logic
programming and implementing type analysis, to parsing natural
language and performing case analysis for algebraic data types.
However, naive implementation is horrifically inefficient. The
inefficiencies are not due to mere constant factors, but rather
unification plays on the boundary of decidability and the unwary can
easy fall prey to a number of asymptotic inefficiencies. These
inefficiencies and many optimizations to avoid them are well-known
within the community, but this knowledge is folklore and seldom
written down or taught. I will be sharing some of these folklore
techniques, as well as a few optimizations which are (to my knowledge)
novel.

