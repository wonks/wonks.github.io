--- 
layout:  post 
title:   "Lifting and Flattening of Typed ASTs"
authors: "Ed Amsden" 
date:    2013-04-26 04:15:00 
categories: Amsden Spring2013
--- 
## Abstract

Strongly-typed functional languages such as Haskell have several
advantages as languages for language implementation. In particular, Algebraic Datatypes
with pattern-matching present a natural way to write much of the functionality of the compiler
or interpreter in an inductive way. Generalized Algebraic Datatypes allow the typing features of the host
language to be employed to ensure that transformations of the AST preserve some notion of
type soundness on the AST.

A useful pattern in language implementation is "flattening", where nested expressions in an AST
are converted to a spine of let-bindings of AST primitives, whose sub-expressions are variable
references brought into scope by the let bindings. I show how to implement a flattening transformation
from a typed AST to a new datatype which preserves the type-soundness of the AST while guaranteeing
by its structure that no nested expressions are present. This permits the user to write total functions over the
AST which are checked for the preservation of AST type-soundness and assume a flattened representation.

