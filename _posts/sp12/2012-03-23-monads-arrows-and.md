--- 
layout:  post 
title:   "Monads, Arrows, and Applicative Functors"
authors: "Rebecca Swords" 
date:    2012-03-23 04:15:00 
categories: Swords Spring2012
--- 
## Abstract

These three mythical beasts each provide a different interface for
composing (possibly effectful) computations. In the presence of side
effects, they also give us a way to identify code that may be
"infected" by these
effects. What exactly is the relationship between these three
concepts? What characteristics differentiate monads from arrows and
applicative functors (also known as idioms), and why would we want to
have all three?

In order to actually use a monad, arrow, or applicative functor, we
have to have a concrete instance: for example, the State or Maybe
monads. Each instantiation must obey certain laws in order to qualify
as a valid
implementation. What are these laws? More importantly, given one of
these concrete instantiations for a monad, can we translate it into an
instance of an arrow or applicative functor, or vice versa?

I will be giving an introduction to monads, arrows, and applicative
functors; discussing the relationships between the three; and offering
answers to the questions posed above.

