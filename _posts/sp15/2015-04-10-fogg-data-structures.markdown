--- 
layout:  post 
title:   "Adaptively Scalable Data Structures"
authors: "Peter Fogg" 
date:    2015-04-10 04:15:00 
categories: Fogg DataStructures Haskell Spring2015
--- 
## Abstract

Purely functional data structures stored inside a mutable variable provide an
excellent concurrent data structure—obviously correct, cheap to create, and
supporting snapshots. They are not, however, scalable. We provide a way to
retain the benefits of these pure-in-a-box data structures while dynamically
converting to a more scalable lock-free data structure under contention. Our
solution scales to any pair of pure and lock-free container types, while
retaining lock-freedom. We demonstrate the principle in action on two very
different platforms: first in the Glasgow Haskell Compiler—extending GHC to
support lock-free data structures and introducing a new approach for safe CAS in
a lazy language—and second in Java.
