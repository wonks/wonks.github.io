--- 
layout:  post 
title:   "Some pieces of the Rust object system: extension, overriding, and self"
authors: "Lindsey Kuper" 
date:    2011-09-09 04:45:00 
categories: Kuper Fall2011
--- 
## Abstract

The Rust programming language combines an expressive static type
system with a lightweight, structural, prototype-based object system.
This combination situates it at an unusual point in the language
design space, since almost all prototype-based object systems are
found in dynamically typed languages such as Self and JavaScript.
Implementing a prototype-based object system in a language that tries
to statically guarantee type safety poses an interesting challenge,
since dynamic object extension and method overriding cause the type of
the current object to change at run-time.  In my talk, I'll discuss
how I implemented self-dispatch, object extension, and method
overriding in the Rust compiler, and explain how these features
interact with each other in ways that I didn't anticipate when I
started the project.

