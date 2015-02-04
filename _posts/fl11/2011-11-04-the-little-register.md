--- 
layout:  post 
title:   "The Little Register Allocator"
authors: "Yin Wang" 
date:    2011-11-04 04:15:00 
categories: Wang Fall2011
--- 
## Abstract

Register allocation has long been formulated as a graph coloring problem,
coloring the dependency graph with physical registers. Such a formulation does
not fully capture the goal of the allocation, which is to minimize the traffic
between registers and memory. Minimizing the number of allocated registers, the
goal of graph coloring, is an imperfect proxy for the real goal.

Following this observation, I propose a register allocation algorithm
by using a kind of flow analysis. The resulting register allocator
directly aims at reducing register-memory traffic, naturally includes
features such as live range splitting, while significantly simplifies
the compiler -- it reduces nine of the back-end passes of my nanopass
compiler into just two.

I will also draw connections to graph coloring and linear scan
register allocation and provide a unified view of register allocation.

