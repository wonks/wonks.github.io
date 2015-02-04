--- 
layout:  post 
title:   "Region-based Memory Management for GPU Programming Languages: Enabling Rich Data Structures on a Spartan Host"
authors: "Eric Holk" 
date:    2014-10-10 04:15:00 
categories: Holk Fall2014
--- 
## Abstract

Graphics Processing Units (GPUs) can effectively accelerate many applications,
but their applicability has been largely limited to problems whose solutions can
be expressed neatly in terms of linear algebra. Indeed, most GPU programming
languages limit the user to simple data structures–typically only
multidimensional rectangular arrays of scalar values. Many algorithms are more
naturally expressed using higher level language features, such as algebraic data
types (ADTs) and first class procedures, yet building these structures in a
manner suitable for a GPU remains a challenge. We present a region-based memory
management approach that enables rich data structures in Harlan, a language for
data parallel computing. Regions enable rich data structures by providing a
uniform representation for pointers on both the CPU and GPU and by providing a
means of transferring entire data structures between CPU and GPU memory. We
demonstrate Harlan’s increased expressiveness on several example programs and
show that Harlan performs well on more traditional data-parallel problems.



