--- 
layout:  post 
title:   "Graph Partitioning For Fun and Profit"
authors: "Chris Wailes" 
date:    2015-11-20 04:15:00 
categories: Wailes Fall2015
--- 
## Abstract

Many load balancing techniques utilize graph representations of tasks and their
communication patters.  The properties of these graphs and the characteristics
of interest heavily impact the design and implementation of the underlying
algorithms.  To successfully evaluate the design space of these algorithms a
generic, composable, and performant library is needed.  In this talk I present
the Task Scales library, the new Normalized Weight algorithm I have developed
(along with it's supporting data structures), and the abstract model that
supports the relational partitioning necessary for topologically aware load
balancing.
