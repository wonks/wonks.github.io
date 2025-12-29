--- 
layout:  post 
title:   "Towards Structural Version Control"
authors: "Yin Wang" 
date:    2012-02-10 04:15:00 
categories: Wang Spring2012
--- 

[**Slides**](https://web.archive.org/web/20131030000419/http://www.cs.indiana.edu/~yw21/slides/ydiff-slides.pdf)

## Abstract

In this talk, I will discuss the design of a structural comparison
tool for programs which compare programs not by their text, but by
their parse tree structures. I will give demos for structural editing
and structural comparison. I will talk about their design space and
the algorithms used in structural comparison: Tree Editing Distance,
Substructure Extraction. I will show how to implement those algorithms
with simple and efficient functional programs. I will also discuss the
design of a parser combinator library in Scheme, and the lessons
learned from my experience of writing parsers for JavaScript and C++.
In the end, I will propose a design of a structural version control
system based on the ideas of structural comparison.



