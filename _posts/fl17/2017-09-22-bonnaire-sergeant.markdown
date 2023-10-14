--- 
layout:  post 
title:   "Space-Efficient Runtime Tracking"
authors: "Ambrose Bonnaire-Sergeant"
date:    2017-09-22 04:15:00
categories: Bonnaire-Sergeant Fall2017
--- 

<iframe width="640" height="320" src="https://www.youtube.com/embed/g5GMQPI8wmw" frameborder="0" allowfullscreen></iframe>

## Abstract

Using an optional type system requires significant manual
effort in the form of writing type annotations. We have implemented
a tool to automatically generate these annotations. Our approach observes
and collects data about a running program, which we combine and
summarize in the form of type annotations.

The naive approach to observing running programs is expensive.
In this talk, we present some key optimizations analogous to space-efficient
gradual typing that significantly reduces this expense, with minor tradeoffs
in annotation accuracy.

[Slides](http://wonks.github.io/slides/bonnaire-sergeant-sept-22nd-2017.pdf)
