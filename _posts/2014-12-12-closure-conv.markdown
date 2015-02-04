--- 
layout:  post 
title:   "The Essence of Closure Conversion"
authors: "Jeremy Siek" 
date:    2014-12-12 04:15:00 
categories: Siek Fall2014
--- 
## Abstract

The interaction between lexical scoping of variables and first-class functions,
as found in all functional programming languages, is rather subtle and
interesting, especially if you want to compile the language to assembly code.
For some reason, computer architects have yet to include first-class functions
with lexical scoping in modern computers! In this talk I'll try to capture the
essence of compiling from a language with lexical scoping and first-class
functions to a language without lexical scoping (but unusually, still with
first-class functions).
