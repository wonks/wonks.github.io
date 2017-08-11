--- 
layout:  post 
title:   "An LCF-Style Tactic Language in Racket's Macro Expander"
authors: "David Christiansen" 
date:    2017-04-07 04:15:00 
categories: Christiansen Spring2017
--- 

## Abstract

A first step in the development of Pudding, a Nuprl-inspired proof system for and in Racket, is to construct a suitable tactic language.
Because much of Racket is defined using macros, reasoning about real Racket programs requires macro expansion. Thus, we must perform this reasoning in the macro expander. Running proofs in the macro expander presents opportunities in addition to challenges: we can re-use the hygiene system to implement bindings, we inherit the DrRacket IDE, and we can both define logics and automate proofs using Racket's metaprogramming tools.

