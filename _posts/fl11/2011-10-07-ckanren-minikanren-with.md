--- 
layout:  post 
title:   "cKanren: miniKanren with Constraints"
authors: "Claire Alvis" 
date:    2011-10-07 04:15:00 
categories: Alvis Fall2011
--- 
## Abstract

We present cKanren, a framework for constraint logic programming (CLP) in
Scheme. cKanren allows programmers to easily define, combine, and use different
kinds of constraints. cKanren includes constraints over finite domains and
disequality constraints over tree terms. cKanren subsumes miniKanren, a logic
programming language embedded in Scheme.  The cKanren framework is designed to
encourage an especially pure style of logic programming in which goals can be
reordered arbitrarily without affecting a program's semantics (with an
important decidability-related caveat).  We develop the complete implementation
of the cKanren framework, written in R6RS Scheme extended with SRFI-39
parameters. We provide the implementation of cKanren's finite domain and
disequality constraint solvers. In addition to these implementations, we provide
introductions to miniKanren and cKanren, and numerous example programs,
including the *Send More Money* cryptarithmetic puzzle and *Eight Queens*.

