--- 
layout:  post 
title:   "Introduction to K: An Executable Semantic Framework"
authors: "Kyle Blocher" 
date:    2012-04-09 04:15:00 
categories: Blocher Spring2012
--- 
## Abstract

K is a rewrite-based executable semantic framework in which
programming languages, type systems and formal analysis tools can be
defined using configurations, computations and rules. Configurations
organize the state in units called cells, which are labeled and can be
nested. Computations carry computational meaning as special nested
list structures sequentializing computational tasks, such as fragments
of program. Computations extend the original language abstract syntax.
K (rewrite) rules make it explicit which parts of the term they
read-only, write-only, read-write, or do not care about. This makes K
suitable for defining truly concurrent languages even in the presence
of sharing. Computations are like any other terms in a rewriting
environment: they can be matched, moved from one place to another,
modified, or deleted. This makes K suitable for defining
control-intensive features such as abrupt termination, exceptions or
call/cc.

