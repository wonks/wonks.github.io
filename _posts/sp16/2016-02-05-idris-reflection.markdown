--- 
layout:  post 
title:   "Reflecting the Idris Elaborator"
authors: "David Christiansen" 
date:    2016-02-05 04:15:00 
categories: Christiansen Idris Spring2016
--- 

## Abstract

Idris is a functional programming language with full dependent types defined by
elaboration to a much simpler core language. In this talk, I will introduce and
discuss two of Idris's metaprogramming features: quasiquotation, which allows
programmers to conveniently represent the core language in Idris source code,
and elaborator reflection, which exposes the internal operations of the
elaboration system to Idris programmers for proof automation and
metaprogramming.

Because dependent types are not yet ubiquitous, this talk will also include a
brief review of dependently typed programming in Idris.
