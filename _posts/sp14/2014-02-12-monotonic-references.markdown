--- 
layout:  post 
title:   "Derailer: Interactive Security Analysis for Web Applications"
authors: "Joe Near" 
date:    2014-09-05 04:15:00 
categories: Securirty Spring2014
--- 
## Abstract

==== Feb. 12: Monotonic References for Gradual Typing ====

Speaker: Jeremy Siek

Abstract:

Gradual type systems enable the use of both static and dynamic type
checking within a single program.  In such systems, it is important to
enable the seemless transfer of data between the static and dynamic
parts of the program while at the same time ensuring that the dynamic
parts do not invalidate the invariants assumed by the static parts.
In particular, dereferencing something of static type 'reference to
integer' should return an integer value. To date, the only approach
that ensured this invariant also induced extra run-time overhead in
every dereference, both in dynamically and statically typed code. In
this talk I present a new point in the design space, monotonic
references, that removes the run-time overhead from dereferencing
statically-typed references. I also give an overview of our proof of
type safety in Isabelle, which was non-trivial because this design
utilizes strong (type-changing) updates to the heap.

