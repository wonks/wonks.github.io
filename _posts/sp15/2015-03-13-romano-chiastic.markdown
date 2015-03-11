--- 
layout:  post 
title:   "Chiastic Lambda-Calculi" 
authors: "Wren Romano" 
date:    2015-03-13 04:15:00 
categories: Romano Spring2015
--- 
## Abstract

In my dissertation I develop a family of calculi: *chiastic lambda-calculi*,
which can be used to capture the syntax and semantics of natural languages with
so-called "free word order" (i.e., where we can rearrange phrases without
altering a sentence's propositional content). Although originally motivated by
linguistic concerns, chiastic lambda-calculi are of independent interest to PL
theory. They provide a type system for first-class keyword-arguments, and/or
first-class named-records. They provide a syntactic justification for informal
notational shorthands in category theory. They provide a perspective on the
distinction between "values" and "computations"--- drawing (novel?) connections
between monads, material set theories, staged computation, and laziness.

On friday, I'll give an introduction to chiastic lambda-calculi; in particular,
to the simply-typed left-chiastic lambda-calculus with full-beta reduction. All
the aforementioned is prior art, presented at NLCS 2013 and at the logic seminar
last November. Instead of re-hashing the same old talk, I'd much rather have a
conversation about my more recent thoughts. In particular, the calculus
discussed at NLCS 2013 does not include eta-conversion, and adding eta is far
from trivial. Sure, we want eta for the usual reasons, but more particularly
adding eta would help to significantly reduce the complexity of the language's
normal forms. So, after giving the introduction, hopefully there will be time
left over to talk a bit about eta.

