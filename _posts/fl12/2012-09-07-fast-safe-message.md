--- 
layout:  post 
title:   "Fast, Safe Message Passing for Rust"
authors: "Eric Holk" 
date:    2012-09-07 04:15:00 
categories: Holk Fall2012
--- 
## Abstract

Rust is a new systems programming language under development at Mozilla.
One of the requirements for Rust’s goal of being safe, concurrent and
practical is an effective message passing system. Such a message passing
system should provide certain correctness guarantees while being amenable
to efficient implementation. I will present a new message passing system
for Rust called pipes. Pipes make use of Rust’s powerful type system and
syntax extension features to enforce that both parties in a communication
session obey a predetermined protocol. These static guarantees allow for
the communicating tasks to synchronize with only one atomic operation in
the best case. In some benchmarks, pipes showed a sevenfold performance
increase over to older port and channel system. Furthermore, pipes provide
a well-defined semantics for ownership of data as it moves between tasks
and enable certain programming patterns that were awkward under the old
port and channel system. My talk will include an introduction to Rust, a
discussion of the design and implementation of the pipes system and an
evaluation of the performance of Pipes.

