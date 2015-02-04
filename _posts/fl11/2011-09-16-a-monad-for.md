--- 
layout:  post 
title:   "A Monad for Deterministic Parallelism"
authors: "Ryan Newton" 
date:    2011-09-16 04:15:00 
categories: Newton Fall2011
--- 
## Abstract

We present a new programming model for deterministic parallel
computation in a pure functional language. The model is monadic and
has explicit granularity, but allows dynamic construction of dataflow
networks that are scheduled at runtime, while remaining deterministic
and pure. The implementation is based on monadic concurrency, which
has until now only been used to simulate concurrency in functional
languages, rather than to provide parallelism. We present the API with
its semantics, and argue that parallel execution is deterministic.
Furthermore, we present a complete work-stealing scheduler implemented
as a Haskell library, and we show that it performs at least as well as
the existing parallel programming models in Haskell.

