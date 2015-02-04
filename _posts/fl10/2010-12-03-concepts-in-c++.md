--- 
layout:  post 
title:   "Concepts in C++"
authors: "Larisse Voufo" 
date:    2010-12-03 04:15:00 
categories: Name Fall2010
--- 
## Abstract

This talk will introduce and motivate my current work on helping further
support for generic programming in C++.
Particularly, the work is on extending the Clang C++ compiler with support
for concepts.

An explicit notion of concepts was supposed to be a major, if not the most
important, addition to the language's
planned new standard: C++0x. However, the feature recently found itself
dramatically voted out,
not for reasons of disagreements on whether to add the feature, but rather
for disagreements on how to add it.
Not even the only working prototype, ConceptGCC, was enough to help
members of the committee reach a consensus...

My work consists of (1) carrying on the vision intended for ConceptGCC,
but from a friendlier and more efficient platform, (2) concretely analyze
the issues that led to this dramatic vote, and (3) determine the right way
to add the feature, for proposal in future planned standards.

In the talk, we will review the ways in which concepts are currently
supported in the language -- which is implicitly,
the various main proposals that were presented to make them explicit
(three), and the ways in which the
prototype implementation could have been more helpful; hence why and how
my current work is intended to complement the previous efforts.



