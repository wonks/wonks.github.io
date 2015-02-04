--- 
layout:  post 
title:   "Closure Optimization"
authors: "R. Kent Dybvig" 
date:    2011-10-21 04:15:00 
categories: Dybvig Fall2011
--- 
## Abstract

First-class procedures, i.e., indefinite extent procedural objects that
retain the values of lexically scoped variables, were incorporated into
the design of the Scheme programming language in 1975 and within a few
years started appearing in functional languages such as ML.  It has taken
many years, but they are fast becoming commonplace, with their inclusion
in contemporary languages such as Javascript.

First-class procedures are often represented at run time as
*closures*.  A closure is a first-class object encapsulating some
representation of a procedure's code (e.g., the starting address of its
machine code) along with some representation of the lexical environment.
In 1984, Cardelli introduced the notion of *flat closures*.  A flat
closure resembles a vector, with a code slot plus one slot for each
free variable.  Flat closures have the useful property that each free
variable is accessible with a single indirect.  They also hold onto no
more of the environment than the procedure might require.

In this talk, I will describe some optimizations of the flat-closure
model that can reduce closure-creation costs and eliminate some
indirects without ever losing the useful features of flat closures.
I will also describe how these optimizations are implemented by Chez
Scheme's compiler.  Some of these optimizations have been performed by
Chez Scheme since 1992, although they have never been published except
in the form of a challenge assignment for a compiler course at Indiana
University.  The remainder have been incorporated only recently.

