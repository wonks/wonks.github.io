--- 
layout:  post 
title:   "Testing specifications of CPU semantics, or, what I did on my summer vacation"
authors: "Lindsey Kuper" 
date:    2010-10-08 04:15:00 
categories: Kuper Fall2010
--- 
## Abstract

Lim & Reps' Transformer Specification Language (TSL) system
comprises a domain-specific programming language for specifying
the semantics of a processor at the level of the instruction set
architecture, together with a run-time system for generating
static analysis engines for executables compiled for that
instruction set.  TSL's ability to generate static analysis
engines from ISA specifications makes it a powerful tool for
analyzing executables, but it's of limited value if the ISA
specifications are wrong in the first place.  We are therefore
interested in verifying the correctness of TSL's ISA
specifications.

In this talk, which presents the work I did this summer in
collaboration with Dave Melski and the research team at
GrammaTech, I will describe how we leverage the TSL system itself
to test TSL's ISA specifications, by generating a CPU *emulator*
that can then be tested in comparison to a physical processor.
I'll cover some of the interesting aspects of the emulator
testing framework we implemented, including a mechanism that
allows the emulator's state to be lazily initialized from a
running Linux process.  Finally, I'll discuss how our emulator
testing framework might be extended to support testing of
*abstract* emulators that have an abstract interpreter at their
core, in addition to the concrete CPU emulators it supports now.

