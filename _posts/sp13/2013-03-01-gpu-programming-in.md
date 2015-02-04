--- 
layout:  post 
title:   "GPU Programming in Rust: Implementing High-level Abstractions in a Systems-level Language"
authors: "Eric Holk" 
date:    2013-03-01 04:15:00 
categories: Holk Spring2013
--- 
## Abstract

Graphics processing units (GPUs) have the potential to greatly accelerate
many applications, yet programming models remain too low level. Many
language-based solutions to date have addressed this problem by creating
embedded domain-specific languages that compile to CUDA or OpenCL. These
targets are meant for human programmers and thus are less than ideal
compilation targets. LLVM recently gained a compilation target for PTX,
NVIDIA's low-level virtual instruction set for GPUs. This lower-level
representation is more expressive than CUDA and OpenCL, making it easier to
support advanced language features such as abstract data types or even
certain closures. We demonstrate the effectiveness of this approach by
extending the Rust programming language with support for GPU kernels. At
the most basic level, our extensions provide functionality that is similar
to that of CUDA. However, our approach seamlessly integrates with many of
Rust's features, making it easy to build a library of ergonomic
abstractions for data parallel computing. This approach provides the
expressiveness of a high level GPU language like Copperhead or Accelerate,
yet also provides the programmer the power needed to create new
abstractions when those we have provided are insufficient.

