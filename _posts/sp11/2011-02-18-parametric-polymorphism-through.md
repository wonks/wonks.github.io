--- 
layout:  post 
title:   "Parametric polymorphism through run-time sealing, or, theorems for low, low prices!"
authors: "Lindsey Kuper" 
date:    2011-02-18 04:15:00 
categories: Kuper Spring2011
--- 
## Abstract

Languages with parametric polymorphism provide the
compile-time guarantee that programs behave uniformly regardless of
the types they are instantiated with.  In such languages, this
parametricity guarantee forms the basis of data abstraction and makes
possible Wadler's "theorems for free!"  In this talk, I'll show how we
can extend System F's parametricity guarantee to a
Matthews-Findler-style multi-language system that combines System F
with a Scheme-like language by use of dynamic sealing, which enforces
data abstraction by using uniquely generated keys to seal values that
should be kept opaque.  While the use of sealing for this purpose has
been suggested before, it has not previously been shown to preserve
parametricity.  Our proof employs a cross-language, step-indexed
logical relation that uses possible worlds to capture the semantics of
seal generation.  Using this possible-worlds model, we can show two
results: first, that System F's parametricity guarantee is preserved
when interoperating with Scheme, and, second, that parametricity is
preserved in a Scheme-only setting that interacts with System F only
to implement a polymorphic contract system.  (This talk describes
current research being done in collaboration with Amal Ahmed and Jacob
Matthews that expands on the work presented in their ESOP 2008 paper
of the same title.)

