--- 
layout:  post 
title:   "Typed Clojure: From Optional to Gradual Typing"
authors: "Ambrose Bonnaire-Sergeant" 
date:    2015-09-11 04:15:00 
categories: Bonnaire-Sergeant Fall2015
--- 
## Abstract

Optional type systems enable type checking for otherwise untyped languages, but
what happens when you need to interact with untyped libraries? In most systems,
the user provides an unchecked annotation which the type system assumes correct.
An incorrect annotation then compromises all guarantees of the type system.

Gradual typing addresses this by inserting dynamic checks that protect the
static invariants of typed code. In this talk we present extensions to Typed
Clojure promoting it from an Optional to a Gradual typing system.
