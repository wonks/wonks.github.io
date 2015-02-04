--- 
layout:  post 
title:   "The Lollipop Guild: Linear Logic and Interactive Fiction"
authors: "Zach Sparks" 
date:    2011-11-11 04:15:00 
categories: Sparks Fall2011
--- 
## Abstract

Well-known interactive fiction writers (including
http://en.wikipedia.org/wiki/Andrew_Plotkin), have argued that a rule-based
approach to writing interactive fiction, as opposed to the current,
object-oriented approach, is a natural way of thinking about writing interactive
fiction. Unfortunately, vanilla logic programming is unable to conveniently deal
with some of the situations that come up frequently when writing interactive
fiction, such as state and exceptions to rules.

One way of dealing with state is to use linear logic programming
rather than vanilla logic programming. Just as propositional logic is
the logic of (simple) knowledge, linear logic is the logic of
consumable resources---each assumption must be used exactly once,
rather than being duplicated or erased at will. I will give an
introduction to linear logic and linear logic programming and follow
it up with some examples of it is applicable to writing interactive
fiction.

