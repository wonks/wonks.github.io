--- 
layout:  post 
title:   "Monotonic References for Efficient Gradual Typing"
authors: "Jeremy Siek" 
date:    2015-04-03 04:15:00 
categories: Siek Monotonic Gradual Spring2015
--- 
## Abstract

Gradual typing enables both static and dynamic typing in the same
program and makes it convenient to migrate code regions between the
two typing disciplines.  One goal of gradual typing is to provide all
the benefits of static typing, such as efficiency, in statically-typed
regions. However, this goal is elusive: the standard approach to
mutable references imposes run-time overhead in statically-typed
regions and alternative approaches are too conservative, either
statically or at run-time. In this paper we present a new semantics
called \emph{monotonic references} which imposes none of the run-time
overhead of dynamic typing in statically typed regions.  With this
design, casting a reference may cause a heap cell to become more
statically typed (but not less). Retaining type safety is challenging
with strong updates to the heap.  Nevertheless, we have a mechanized
proof of type safety. Further, we present blame tracking for monotonic
references and prove a blame theorem.
