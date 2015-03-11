--- 
layout:  post 
title:   "Running Typed Racket Backwards" 
authors: "Ambrose Bonnaire-Sergeant" 
date:    2015-03-06 04:15:00 
categories: Bonnaire-Sergeant Spring2015
--- 
## Abstract

Typed Racket can type check typical Racket programs via occurrence typing, which
uses information collected at conditional tests to refine types down conditional
branches. We introduce the fundamentals of occurrence typing and then see what
programs an implementation of occurrence typing in miniKanren can check (and
generate!).
