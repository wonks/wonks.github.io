--- 
layout:  post 
title:   "Enhancing work-stealing runtimes with concurrency"
authors: "Chris Zakian and Tim Zakian" 
date:    2013-03-29 04:15:00 
categories: Zakian Spring2013
--- 
## Abstract

Parallelism and concurrency are both important to modern programming.
Applications need to use multiple cores by exposing independent
computations (parallelism), and they also need to perform IO, including blocking
operations that require non-deterministically interleaved threads of control
(concurrency).  Many libraries for parallelism in C++ are now available
(TBB, TPL, Cilk), as well as libraries for lightweight user threading
(Qthreads), but no existing systems combine these benefits effectively: i.e. allowing
full composability of task-spawning and blocking within programs.

In this paper, we argue that the solution is to enhance existing
work-stealing
parallel runtimes to become lightweight threading systems as well.  We
demonstrate this approach by extending Intel Cilk Plus with cooperative
threading capabilities (blocked computations).  Our solution increases the
code size of the Cilk runtime by less than five percent, and imposes very
low overhead for Cilk programs that do not use concurrency features.
The new concurrency features have lower context-switching overhead than
Pthreads, and are comparable to other languages supporting user-level
threads.

