--- 
layout:  post 
title:   "ICFP 2016 Practice Talks II"
authors  "Wazim Mohammed Ismail, Trevor L. McDonell" 
date:    2016-09-09 04:15:00 
categories: McDonell Ismael Fall2016
--- 

This Friday, we're going to have two back-to-back practice talks. Please attend
to provide feedback, commentary, and the like.

# Deriving a probability density calculator (Functional pearl)

*Wazim Mohammed Ismail*

Given an expression that denotes a probability distribution, often we want a
corresponding density function, to use in probabilistic inference. Fortunately,
the task of finding a density has been automated.  It turns out that we can
derive a compositional procedure for finding a density, by equational reasoning
about integrals, starting with the mathematical specification of what a density
is. Moreover, the density found can be run as an estimation algorithm, as well
as simplified as an exact formula to improve the estimate.

# Ghostbuster: A Tool for Simplifying and Converting GADTs

*Trevor L. McDonell*

Generalized Algebraic Dataypes, or simply GADTs, can encode non-trivial
properties in the types of the constructors. Once such properties are encoded in
a datatype, however, all code manipulating that datatype must provide proof that
it maintains these properties in order to typecheck. In this paper, we take a
step towards gradualizing these obligations. We introduce a tool, Ghostbuster,
that produces simplified versions of GADTs which elide selected type parameters,
thereby weakening the guarantees of the simplified datatype in exchange for
reducing the obligations necessary to manipulate it. Like ornaments, these
simplified datatypes preserve the recursive structure of the original, but
unlike ornaments we focus on information-preserving bidirectional
transformations. Ghostbuster generates type-safe conversion functions between
the original and simplified datatypes, which we prove are the identity function
when composed. We evaluate a prototype tool for Haskell against thousands of
GADTs found on the Hackage package database, generating simpler Haskell’98
datatypes and round-trip conversion functions between the two.
