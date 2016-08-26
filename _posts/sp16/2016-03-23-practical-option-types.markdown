--- 
layout:  post 
title:   "Practical Optional Types for Clojure"
authors: "Ambrose Bonnaire-Sergeant"
date:    2016-03-23 04:15:00 
categories: Bonnaire-Sergeant Spring2016
--- 

## Abstract

*(ESOP practice talk, 25+5m)*

Typed Clojure is an optional type system for Clojure, a dynamic language in the
Lisp family that targets the JVM. Typed Clojure enables Clojure programmers to
gain greater confidence in the correctness of their code via static type
checking while remaining in the Clojure world, and has acquired significant
adoption in the Clojure community. Typed Clojure repurposes Typed Racket’s
occurrence typing, an approach to statically reasoning about predicate tests,
and also includes several new type system features to handle existing Clojure
idioms.

In this talk we introduce Typed Clojure and demonstrate a selection of key ideas
behind its design.
