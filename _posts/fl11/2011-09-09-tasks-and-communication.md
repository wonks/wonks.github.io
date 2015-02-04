--- 
layout:  post 
title:   "Tasks and Communication in Rust"
authors: "Eric Holk" 
date:    2011-09-09 04:15:00 
categories: Holk Fall2011
--- 
## Abstract

Rust is a new programming language for systems software under
development at Mozilla. Rust aims to be safe, concurrent, practical
and fast, and accomplishes this through standard techniques such as a
type system that enforces memory techniques, but also with more
uncommon features such as a typestate system. Particular attention is
given to allowing the programmer control over where objects reside in
memory and tracking ownership as values move through a program. These
features allow Rust's task and communication system to be expressed
completely as a library instead of requiring additional language
primitives, simplifying the overall language design and
implementation. I'll be providing a brief overview of the Rust
language, and focus on my work implementing the task and communication
system this summer.

