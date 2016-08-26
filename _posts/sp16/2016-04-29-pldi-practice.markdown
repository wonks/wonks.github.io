--- 
layout:  post 
title:   "Two PLDI Practice Talks (see description)"
authors: "Buddhika Chamith and Andrew Kent"
date:    2016-04-29 04:15:00 
categories: Kent Chamith Spring2016
--- 

This Friday, we will have *two* practice talks for accepted PLDI papers.

# Living on the edge: Rapid-toggling probes with cross modification on x86

Author: Buddhika Chamith

Dynamic probe injection is now a widely used method to de- bug performance in
production. Current techniques for dynamic probing of native code, however, rely
on an expensive stop-the-world approach: binary changes are made within a safe
state of the program—typically in which all the program threads are halted—to
ensure that another thread executing the modified code region doesn’t step into
a partially modified code. Stop-the-world patching is not scalable. In contrast,
low overhead, scalable probes that can be rapidly toggled on and off in-place
would open up new use cases for statistical profilers and language
implementations, even traditional ahead of time, native code compilers. In this
talk I will describe safe cross-modification protocols that mutate x86 code
between threads but do not require quiescing threads, resulting in radically
lower overheads than existing solutions. A key problem is handling instructions
that straddle cache lines. We empirically evaluate existing x86 architectures to
derive a safe policy given current processor behavior, and we argue that future
architectures should clarify the semantics of instruction fetching to make cheap
cross-modification easier and future proof.


# Occurrence Typing Modulo Theories

Author: Andrew Kent

We present a new type system combining occurrence typing---a technique
previously used to type check programs in dynamically-typed languages such as
Racket, Clojure, and JavaScript---with dependent refinement types. We
demonstrate that the addition of refinement types allows the integration of
arbitrary solver-backed reasoning about logical propositions from external
theories. By building on occurrence typing, we can add our enriched type system
as a natural extension of Typed Racket, reusing its core while increasing its
expressiveness. The result is a well-tested type system with a conservative,
decidable core in which types may depend on a small but extensible set of
program terms.
