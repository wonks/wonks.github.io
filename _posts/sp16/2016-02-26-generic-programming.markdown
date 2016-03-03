--- 
layout:  post 
title:   "Generic Programming for the Masses"
authors: "Ryan Scott" 
date:    2016-02-26 04:15:00 
categories: Scott Haskell Spring2016
--- 

## Abstract

Generic programming is a technique for writing code that is reusable for many
different datatypes. This is an effective technique for eliminating boilerplate
code, and many programming languages have at least some support for writing
generic programs. However, most languages fall flat in that either (1) their
generic programming capabilities are limited to a few built-in (i.e., magical)
functions, or (2) rely on a heavyweight macro system that makes it difficult to
write generic programs in a cheap and cheerful way.

In this talk, I present an alternative generic programming mechanism found in
the Glasgow Haskell Compiler (GHC), referred to as GHC Generics. GHC's approach
greatly simplifies the effort needed to write generic programs and requires
almost no compiler magic. We explore how GHC Generics makes it possible to write
polytypic code by viewing any algebraic data type as a polynomial functor. We
also discuss the tradeoffs involved when using GHC Generics as opposed to other
generic programming techniques.
