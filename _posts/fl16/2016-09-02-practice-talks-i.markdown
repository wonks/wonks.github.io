--- 
layout:  post 
title:   "ICFP 2016 Practice Talks I"
authors:  "David Christiansen, Jason Hemann" 
date:    2016-09-02 04:15:00 
categories: Christiansen Hemann Fall2016
--- 

This Friday, we're going to have two back-to-back practice talks. Please attend
to provide feedback, commentary, and the like.

# Elaborator Reflection: Extending Idris in Idris

*David Christiansen*

Many programming languages and proof assistants are defined by
elaboration from a high-level language with a great deal of implicit
information to a highly explicit core language. In many advanced
languages, these elaboration facilities contain powerful tools for
program construction, but these tools are rarely designed to be
repurposed by users. We describe elaborator reflection , a paradigm for
metaprogramming in which the elaboration machinery is made directly
available to metaprograms, as well as a concrete realization of
elaborator reflection in Idris, a functional language with full
dependent types. We demonstrate the applicability of Idris’s reflected
elaboration framework to a number of realistic problems, we discuss the
motivation for the specific features of its design, and we explore the
broader meaning of elaborator reflection as it can relate to other
languages.

# A Framework for Extending microKanren with Constraints

*Jason Hemann*

We present a framework for building CLP languages with symbolic
constraints based on microKanren, a domain-specific logic language
shallowly embedded in Racket. A language designer provides the names
and violation conditions of atomic constraints. We rely on Racket's
macro system to generate a black-box constraint solver and other
components of the microKanren embedding. The framework itself and the
implementation of common Kanren constraints amounts to just over 100
lines of code. Our framework is both a teachable implementation for
constraint logic programming as well as a test-bed and prototyping tool
for constraint systems.
