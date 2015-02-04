--- 
layout:  post 
title:   "Towards a Computational Account of Homotopy Type Theory"
authors: "Zach Sparks" 
date:    2014-01-31 04:15:00 
categories: Sparks HoTT Spring2014
--- 
## Abstract

Homotopy type theory (HoTT) has recently become a popular topic of discussion in
certain circles in PL academia, drawing from research in programming languages,
topology, and category theory. Its main focus is equality of elements, and
specifically looking at paths between equal objects. Unfortunately, they
currently must postulate that types have a path between them (ie, are equal)
exactly when there is an equivalence between them. This axiom---known as the
univalence axiom---is aesthetically unpleasing to some, and also causes
difficulties when trying to interpret HoTT as a programming language with
computational rules.

The Pi programming language is a language in which all computations are
reversible. This provides a natural setting for reasoning about equality, since
the type of programs in Pi forms an equivalence relation by design. Together
with Amr Sabry and Jacques Carette, I have been working on a computational
alternative to HoTT, using Pi as a basis. In this talk, I will introduce the
basics of both HoTT and Pi, explain the problems with HoTT, and discuss our
novel approach to solving them.

