--- 
layout:  post 
title:   "Refined Criteria for Gradual Typing" 
authors: "Jeremy Siek" 
date:    2015-01-29 04:15:00 
categories: GradualTyping Siek Spring2015
--- 
## Abstract

Siek and Taha [2006] coined the term gradual typing to describe
a technical approach to integrating static and dynamic typing within a
single language that 1) puts the programmer in control of which
regions of code are statically or dynamically typed, and 2) enables
the gradual migration of code between the two typing
disciplines. Since 2006, the term gradual typing has become
quite popular but its meaning has become diluted to encompass anything
related to the integration of static and dynamic typing. This dilution
is partly the fault of the original paper, which provided an
incomplete formal characterization of what it means to be gradually
typed. In this talk I draw a crisp line in the sand,
articulating a new formal property, named the gradual
guarantee, that relates the behavior of programs that differ only
with respect to the precision of their type annotations.  I argue
that the gradual guarantee provides important guidance for designers
of gradually-typed languages. I survey the gradual typing literature,
critiquing designs in light of the gradual guarantee. I report on a
mechanized proof that the gradual guarantee holds for the
Gradually-Typed Lambda Calculus.
   
