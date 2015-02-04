--- 
layout:  post 
title:   "Declarative Parallel Programming"
authors: "Will Byrd" 
date:    2012-02-24 04:15:00 
categories: Byrd Spring2012
--- 
## Abstract

Declarative languages allow programmers to specify *what* a program should do,
without specifying *how* to do it.  Expressing the *what*, and leaving
the *how* to the compiler and runtime system, leads to shorter, simpler,
and safer programs.  The declarative approach is especially promising for
difficult programming tasks, which is why declarative programming has been
popular in artificial intelligence research for decades.  One notoriously
difficult task is the programming of multi-core and multi-processor computers,
which are now found not only in supercomputers, but also laptops, cell phones,
and gaming consoles.  Graphics processors (GPUs) are essentially parallel
supercomputers, and are also difficult to program.  The recent introduction of
hybrid CPU/GPU clusters adds even more complexity.

To address the complexity of programming modern parallel hardware, my colleagues
and I in the Declarative Parallel Programming project at Indiana University are
developing two related declarative languages: Kanor, a language for specifying
collective communication on clusters; and Harlan, a language for describing
computational kernels on GPUs and other accelerators.

I will describe how Kanor allows programmers to declaratively, but explicitly,
specify the essence of communication patterns. The programmer lets the
implementation handle the details when appropriate, but retains the option to
hand-encode communications when necessary, providing a balance between
declarativeness and performance predictability and tunability. Similarly, Harlan
allows the user to declaratively, but explicitly, describe computational kernels
and to coordinate computation, data layout, and memory movement. As with Kanor,
this approach gives the programmer enough control to write efficient code, while
abstracting over the low-level details that make GPU programming so difficult.
Integrating Harlan into Kanor results in a unified, high-level, flexible
language suitable for efficiently programming hybrid clusters, traditional
(CPU-based) clusters, and GPUs on a single machine.

