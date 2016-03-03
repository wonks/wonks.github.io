--- 
layout:  post 
title:   "Strong Normalization for Chiastic Lambda-Calculi"
authors: "Wren Romano" 
date:    2016-03-04 04:15:00 
categories: Romano Spring2016
--- 

## Abstract

One of the properties we like in our calculi is strong normalization. One of the
most fruitful techniques for proving strong normalization is Tait's method and
extensions to it, such as Girard's Candidats De Reductibilité, logical
predicates/relations, etc. But what about when the technique doesn't work? For
example, your calculus has a single rule which eliminates multiple connectives.
The folkloric response is “don't do that”, but we cannot always avoid doing so.
Associative and chiastic lambda-calculi require just such a rule. In this talk I
will present Tait's method, explain why it fails for these rules, and then
present a novel(afaik) extension to the method which can handle them.

This is work-in-progress from my dissertation, and the result is less than a
week old(!), so it'll be more of a whiteboard talk than a polished slides-talk.
(Though I will have slides for presenting the syntax and judgement rules, to
avoid too much writing.)

