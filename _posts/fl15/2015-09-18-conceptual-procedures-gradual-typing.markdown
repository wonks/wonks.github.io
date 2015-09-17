--- 
layout:  post 
title:   "A methodology, conceptual procedures and a supporting tool for Gradual Typing"
authors: "Matteo Cimini" 
date:    2015-09-18 04:15:00 
categories: Cimini Spring2015
--- 
## Abstract

Many languages are beginning to integrate dynamic and static typing.
Siek and Taha offered gradual typing as an approach to this
integration that provides the benefits of a coherent and full-span
migration between the two disciplines. However, the literature lacks a
general methodology for designing gradually typed languages.  Our
first contribution is to provide such a methodology insofar as the
static aspects of gradual typing are concerned: deriving the gradual
type system and the compilation to the cast calculus.

Based on this methodology, we present *the Gradualizer*, an algorithm that
generates a gradual type system from a well-formed type system (expressed as a
logic program) and also generates a compiler to the cast calculus. Our algorithm
handles a large class of type systems and generates systems that are correct
with respect to the formal criteria of gradual typing. Finally, we report on an
implementation of the Gradualizer that takes type systems expressed in
$\lambda$-prolog and outputs their gradually typed version (and compiler to the
cast calculus) in $\lambda$-prolog. We also report on ongoing work towards a
methodology for deriving the operational semantics for executing gradual
programs.

