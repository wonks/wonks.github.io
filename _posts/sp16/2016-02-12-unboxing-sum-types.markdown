--- 
layout:  post 
title:   "Unboxing Sum Types in GHC"
authors: "Ömer Sinan Ağacan" 
date:    2016-02-12 04:15:00 
categories: Agacan Haskell Spring2016
--- 

## Abstract

GHC 8.0 moves towards making Haskell programs more strict by introducing two new
language pragmas that transform programs to programs that evaluate more like
programs in a call-by-value language. One nice side-effect of having more strict
programs is that we now need thunks less, and without thunks we don't need
boxing as much as before. GHC already has some compiler passes that optimize
cases where we don't need thunking and boxing, but those optimizations were only
working on values with product types.

This talk will introduce "UnboxedSums", a new GHC extension that adds a new kind
of first-class value (anonymous unboxed sums) to the language that makes more
efficient representation of strict sum types possible. This extension enables
GHC to store strict sum types in "unboxed" form, and by extending existing
"demand analysis" and "constructed product results analysis" passes it makes it
possible for strict functions on sum types to use more efficient calling
conventions (improving both argument passing and returning).

To our knowledge, this feature is novel. While it was always possible to do in
languages with manual memory management, no other garbage-collected language has
this feature and does the optimizations we do on sum types.

### Links

https://github.com/osa1/ghc/tree/unboxed-sums-stg

http://cs.indiana.edu/~rrnewton/temp/ghc-8.1.20160201_ubx_sums_1.2-x86_64-unknown-linux.tar.xz
