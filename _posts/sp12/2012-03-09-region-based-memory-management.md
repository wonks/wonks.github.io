--- 
layout:  post 
title:   "Region-based Memory Management"
authors: "Eric Holk" 
date:    2012-03-09 04:15:00 
categories: Holk Spring2012
--- 
##Abstract

Regions are a means of combining many objects into a single unit of memory
allocation. As a form of memory management, they provide many of the efficiency
benefits of stack allocation, yet regions also provide more flexibility for
objects that outlive their stack frame. Although conceptually simple, regions
have proven useful in a variety of applications. The Apache web server uses
regions to amortize the cost of deallocation for large data structures. Regions
have been used in ML to statically place allocation and deallocation points and
avoid the need for a tracing garbage collector. Cyclone uses regions to
eliminate dangling pointer references.

In my talk, I will provide a brief overview of region-based memory management,
including approaches to region influence. I will discuss how different projects
have used regions to achieve their goals. Finally, I will provide some
speculation on how regions might be used to support richer data structures and
efficient memory movement for GPU computing in Harlan.

