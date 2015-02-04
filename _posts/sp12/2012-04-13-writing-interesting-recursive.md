--- 
layout:  post 
title:   "Writing Interesting Recursive Programs in a (New) Spartan Host"
authors: "Chris Frisz" 
date:    2012-04-13 04:15:00 
categories: Frisz Spring2012
--- 
## Abstract

Tail-call optimization allows programmers to write interesting
tail-recursive functions without worry of overflowing the program's
stack memory. This is achieved by reusing the stack frame of the
calling function for the recursive call. A number of languages, such
as Scheme and Standard ML, require tail-call optimization as part of
their language standards, making tail-recursion a primary means of
iteration in these languages. In this talk we discuss the state of
tail-call optimization in Clojure, a Lisp dialect targeting the JVM.
Specifically, we examine the language's current limitation on
constant-space tail calls that are only available to programmers
through manual code transformations. We then present a method to
extend support for tail-call optimization to arbitrary mutual
recursion via well-known code transformations such as CPS and
trampolining. Finally, we present a prototype for a source-to-source
compiler embedded in Clojure for performing these transformations.

