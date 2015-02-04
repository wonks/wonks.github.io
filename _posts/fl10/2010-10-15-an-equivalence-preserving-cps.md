--- 
layout:  post 
title:   "An Equivalence-Preserving CPS Translation via Multi-Language Semantics"
authors: "Amal Ahmed" 
date:    2010-10-15 04:15:00 
categories: Ahmed Fall2010
--- 
## Abstract

Language-based security relies on the assumption that all potential
attacks follow the rules of the language in question.  When programs
are compiled into a different language, this is true only if the
translation process preserves observational equivalence.

To prove that a translation preserves equivalence, one must show that
if two program fragments cannot be distinguished by any source
context, then their translations cannot be distinguished by any target
context.  Informally, target contexts must be no more powerful than
source contexts, i.e., for every target context there exists a source
context that "behaves the same."  This seems to amount to being able
to "back-translate" arbitrary target terms.  However, that is simply
not viable for practical compilers where the target language is
lower-level and, thus, contains expressions that have no source
equivalent.

In this talk, I'll present a CPS translation from a less expressive
source language (STLC) to a more expressive target language (System F)
and prove that the translation preserves observational equivalence.
The key to our equivalence-preserving compilation is the choice of the
right type translation: a source type T mandates a set of behaviors
and we must ensure that its translation T+ mandates semantically
equivalent behaviors at the target level.  Based on this type
translation, we demonstrate how to prove that for every target term of
type T+, there exists an equivalent source term of type T --- even
when sub-terms of the target term are not necessarily
"back-translatable" themselves.  A key novelty of our proof,
resulting in a pleasant proof structure, is that it leverages a
multi-language semantics where source and target terms may
interoperate.

