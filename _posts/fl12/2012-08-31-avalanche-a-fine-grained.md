--- 
layout:  post 
title:   "Avalanche: A Fine-Grained Flow Graph Model for Irregular Applications on Distributed-Memory Systems"
authors: "Jeremiah Willcock" 
date:    2012-08-31 04:45:00 
categories: Willcock Fall2012
--- 
## Abstract

Flow graph models have recently become increasingly popular as a way to
express parallel computations.  However, most of these models either
require specialized languages and compilers or are library-based solutions
requiring coarse-grained applications to achieve acceptable performance.
Yet, graph algorithms and other irregular applications are increasingly
important to modern high-performance computing, and these applications are
not amenable to coarsening without complicating algorithm structure. One
effective existing approach for these applications relies on active
messages. However, the separation of control flow between the main program
and active message handlers introduces programming difficulties. To
ameliorate this problem, we present Avalanche, a flow graph model for
fine-grained applications that automatically generates active-message
handlers. Avalanche is built as a C++ library on top of our
previously-developed Active Pebbles model; a set of combinators builds
graphs at compile-time, allowing several optimizations to be applied by
the library and a standard C++ compiler.  In particular, consecutive flow
graph nodes can be fused; experimental results show that flow graphs built
from small components can still efficiently operate on fine-grained data.

