--- 
layout:  post 
title:   "Co-dfns Compiler Architecture"
authors: "Aaron Hsu"
date:    2016-04-01 04:15:00 
categories: Hsu Spring2016
--- 

## Abstract

In this casual talk, I would like to discuss my increasingly specific
preferences and designs that have developed around the Co-dfns compiler
architecture. The specific and intentional design constraints lead to an
interesting set of programming practices that differ from conventional
wisdom, but which tend to increase the manageability of the source code.
Furthermore, I will provide a broader perspective on array programming of
this sort, how it connects with traditional themes that appear in the array
programming community, how they differ, and thoughts on their general
applicability to wider domains. Particular emphasis will be put on the
pervasive use of trains-based points-free style programming, idioms use
versus function/object abstraction, flat namespaces and "flat" dependency
chains, and a particular set of techniques used to make array programming
and data-parallel programming in particular fit well with the needs of
the compiler writer.
