--- 
layout:  post 
title:   "Rethinking Loops as Infinite State Transducers"
authors: "Adit Shah" 
date:    2015-09-25 04:15:00 
categories: Shah Transducers Fall2015
--- 
## Abstract

Traditional loop iteration structures, such as for and while, are neither
modular nor composable. However, loop combinators in functional programming
languages, such as map and filter, are both modular and composable.
Unfortunately, loop combinators aren't generic. Hence, you have to create a new
set of loop combinators for each underlying data structure, such as lists and
streams. Transducers, introduced by Rich Hickey for Clojure, are composable
generic data structures which reify a loop. In addition, they can be very
efficient as they enable stream fusion and tail call optimization.
   
In this talk we present a different way of thinking about Clojure transducers.
We show how to import transducers into typed functional programming languages
such as Haskell and OCaml and we demonstrate some of the uses of transducers
which makes programming simpler. Finally, we compare our ideas with related work
in the field. Although our ideas are not novel yet we hope that you take away
some valuable information from our talk.
