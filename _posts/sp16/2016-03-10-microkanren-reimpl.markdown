--- 
layout:  post 
title:   "A Reimplementation of microKanren"
authors: "Jason Hemann"
date:    2016-03-10 04:15:00 
categories: Hemann Spring2016 minikanren
--- 

## Abstract

miniKanren, and microKanren, was designed to be an embedded language in a small
subset of Scheme. This aids developers in transliterating *Kanren to a great
number and variety of other languages (50+), making logic programming available
in many non-traditional environments and helping to bridge a gap between
distinct families of declarative languages.

This shallow embedding enables a "quick and dirty" explanation of the meanings
of our programs -- we explain them in terms of our host language's features.
However, advanced features (e.g., a generic constraint system) and varied host
languages make this solution unsatisfactory.

As such, we require more rigorous and host-independent characterizations of
miniKanren's meanings -- and hopefully at a higher level of abstraction than
source code.

In this talk, I will present our first steps along this path, developing and
demonstrating a reimplementation of microKanren amenable to a host-independent
characterization, and discuss future steps.

