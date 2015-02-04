--- 
layout:  post 
title:   "Implementation of the Nanopass Framework"
authors: "Andrew Keep" 
date:    2010-11-12 04:15:00 
categories: Keep Fall2010
--- 
## Abstract

The goal of the nanopass framework is to provide a simple and
efficient tool for writing compilers composed of small passes.  The
framework provides two macros for defining passes as well as the
intermediate languages used by the passes.  Keeping the interface
simple for compiler writers though, leads to several implementation
challenges.  First, new languages can be defined as extensions to old
languages, meaning language information must be maintained and
transformed at compile time.  Second, passes are written using
s-expression syntax to decompose and construct terms, while the
underlying implementation uses records based on language definitions.
These must be transformed into the appropriate definitions at compile
time.  Third, run-time checking of both incoming and constructed terms
to ensure well-formed language terms at the beginning and end of each
pass.  Finally, to keep pass writing as simple as possible "trivial"
cases, i.e. cases where a term is simply carried along through a pass,
need not be written by the compiler writer, meaning the framework is
responsible for creating them at compile time.  In this talk, I
breifly introduce the syntax and features of the nanopass framework,
and then discuss how we address these challenges in implementing the
macros to support these features.

