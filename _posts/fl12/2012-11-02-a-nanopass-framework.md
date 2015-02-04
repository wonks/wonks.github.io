--- 
layout:  post 
title:   "A Nanopass Framework Tutorial"
authors: "Andrew Keep" 
date:    2012-11-02 04:15:00 
categories: Keep Fall2012
--- 
## Abstract

The nanopass framework is an embedded-DSL for writing compilers in Scheme.  The
idea for the nanopass framework grew out of development of the micropass
compiler, used in the compiler course originated by Dan Friedman and refined by
Kent Dybvig and Oscar Waddell.  The micropass compiler uses S-expressions for
intermediate representation, along with a match form to pattern match input
S-expression language forms and construct output S-expression language forms
from quasiquoted templates.  Writing a compiler in the micropass style makes it
easier to understand the task each pass of the compiler performs.  Using
S-expressions as the intermediate representation has a few downsides.  First,
efficiency can be a problem due to pattern-matching overhead and the need to
rebuild large S-expressions.  Second, passes often contain boilerplate code to
recur through otherwise unchanging language forms.  Third, the S-expression
representation lacks formal structure, and it is possible to create ill-formed
output that might not be caught until several passes later in the compiler.  The
nanopass framework addresses these concerns by providing two main forms
define-language and define-pass.  The define-language form formally specifies
the grammar of an intermediate language.  The define-pass form defines a pass
that operates on one language and produces output in another, possibly
different, language.  The output language forms are constructed in a way that
ensures they match the output language specified by the pass.

The nanopass framework has seen a few iterations.  An initial prototype was
developed by Jordan Johnson.  The paper "A Nanopass Infrastructure for Compiler
Education" by Dipanwita Sarkar, Oscar Waddell, and R. Kent Dybvig (and
subsequently Dr. Sarkar's dissertation) describe a second prototype of nanopass
framework, and its use for educational compiler development.

This tutorial will discuss a new version of the nanopass framework, intended for
the development of commercial compilers.  A nanopass version of the class
compiler will provide examples of how to use the framework, and demonstrate some
of the new features.

