--- 
layout:  post 
title:   "Kanor: A Declarative Language for Explicit Communication"
authors: "Eric Holk" 
date:    2011-01-21 04:15:00 
categories: Holk Spring2011
--- 
## Abstract

Programmers of high-performance applications face two major implementation
options: to use a high-level language which manages communication implicitly or
to use a low-level language while specifying communication explicitly.  The
high-level approach offers safety and convenience, but forces programmers to
give up control, making it difficult to hand-tune communications or to estimate
communication cost.  The low-level approach retains this control, but forces
programmers to express communication at a verbose, tedious, and error-prone
level of detail.

We advocate a complementary third approach in which the programmer
declaratively, but explicitly, specifies the essence of the communication
pattern.  The programmer lets the implementation handle the details when
appropriate, but retains enough control to hand-encode communications when
necessary.  In this paper we present Kanor, a language for declaratively
expressing explicit communication patterns, and demonstrate how Kanor safely,
succinctly, and efficiently expresses both point-to-point and collective
communications.


