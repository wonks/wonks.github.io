--- 
layout:  post 
title:   "Fizz and Fuse Your Arrays"
authors: "Michael Vollmer" 
date:    2015-10-23 04:15:00 
categories: Vollmer Array Optimization Fall2015
--- 
## Abstract

Array fusion is a vital optimization in functional array programming. With array
fusion, functions operating on arrays can be written in a high-level,
compositional style, yet still "fuse" down to a single, efficient loop, with no
need to allocate intermediary arrays. This produces data-parallel code, but
often does not leave any opportunities for task-parallelism. Array fissioning
goes in the opposite direction: single functions are "fizzed" into two or more
chunks. Fission is compatible with fusion, and allows for functional array
programs to be implicitly distributed across multiple devices.

In this talk, I will discuss different functional array representations and
describe how to implement fusion and fissioning.

The presentation slides are available here: http://vollmerm.github.io/FizzFuseArrays/slides.pdf