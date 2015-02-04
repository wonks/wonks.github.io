--- 
layout:  post 
title:   "Bringing Atomic Memory Operations to a Lazy Language"
authors: "Ryan Newton" 
date:    2012-09-21 04:15:00 
categories: Newton Fall2012
--- 
## Abstract

The GHC Haskell compiler recently gained the capability to generate
atomic compare-and-swap (CAS) assembly instructions. This opens up a
new world of data-structure implementation possibilities, but also
raises a number of problems due to the fact that pointer equality is
not, in general, a meaningful concept in Haskell.

This talk describes existing CAS support for IORefs and Arrays and
provide a recipe for others to add additional operations (e.g.
test-and-set, fetch-and-add).  We present performance results for our
implementions of data structures such as Michael-Scott queues and
Chase-Lev work-stealing deques.  Finally, we give guidelines for how
to write code that is robust to Haskell program transformations that
will cause spurious failures of operations like CAS; this includes a
discussion of GHC-specific guarantees (NOINLINE, etc) that enable safe
use of atomic pointer operations.

