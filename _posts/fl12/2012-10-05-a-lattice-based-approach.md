--- 
layout:  post 
title:   "A Lattice-Based Approach to Deterministic Parallelism with Shared State"
authors: "Lindsey Kuper" 
date:    2012-10-05 04:15:00 
categories: Kuper Fall2012
--- 
## Abstract

[Video](http://www.youtube.com/watch?v=jQnklQhgUH0)

Programs written using a deterministic-by-construction model of
parallel computation always produce the same observable results,
offering programmers the promise of freedom from subtle,
hard-to-reproduce nondeterministic bugs.  A common thread that emerges
in the study of deterministic-by-construction systems, from venerable
models like Kahn process networks to modern ones like Intel's
Concurrent Collections system, is that the determinism of the model
hinges on some notion of monotonicity.  Taking monotonicity as a
guiding principle, then, I'll present a new model for deterministic
parallel programming that generalizes existing single-assignment
models to allow multiple assignments that are monotonically increasing
with respect to a user-specified lattice. As I'll show in my talk, this
model achieves determinism by using a shared data structure with an
API that allows only monotonically increasing writes and restricted
reads.  The resulting model also provides a theoretical
grouunding for exploring a limited form of nondeterminism that admits
failures but never wrong answers.


