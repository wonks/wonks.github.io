--- 
layout:  post 
title:   "An Introduction to Dependently Typed Racket"
authors: "Andrew Kent" 
date:    2014-11-14 04:15:00 
categories: Kent Fall2014
--- 
## Abstract

Typed Racket is a gradually typed dialect of Racket that seeks to accommodate
common typed-based reasoning used in untyped languages, while requiring few
changes to the code itself. However, thus far Typed Racket has only supported
formally reasoning about relatively simple types. In this informal talk I will
briefly review the base calculus for this system (λTR) and illustrate how
decidable dependent types (such as those found in Dependent ML) are a natural
extension to the calculus.
