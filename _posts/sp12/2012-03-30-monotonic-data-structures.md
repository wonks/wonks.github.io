--- 
layout:  post 
title:   "Monotonic data structures as a guiding principle for deterministic parallel programming"
authors: "Lindsey Kuper" 
date:    2012-03-30 04:15:00 
categories: Kuper Spring2012
--- 
## Abstract

Kahn process networks, Haskell's monad-par library, and Intel's
Concurrent Collections language are three diverse examples of
deterministic-by-construction models of parallel computation.  In a
deterministic-by-construction model, all programs written using the
model are guaranteed to behave deterministically, so they offer
programmers the promise of freedom from subtle, hard-to-reproduce
nondeterministic bugs like race conditions.

As I'll show in my talk, the determinism of all of these models hinges
on a notion of *monotonic data structures*---data structures in which
mutators may only add information, never destroy it.  In each case, a
monotonicity property on some data structure captures the essence
of *why* the model is deterministic.  With monotonic data structures
as a guiding principle, then, we should be able to develop a
deterministic parallel programming model that is general enough to
express existing models, as well as guide the design of new ones.
Ryan Newton, Amr Sabry, and I are working on developing such a model,
and I'll discuss what we've accomplished so far and where we're headed
next.  (Warning to implementors: this talk may contain theorems and
inference rules!  Warning to theorists: this talk may contain running
code!)

