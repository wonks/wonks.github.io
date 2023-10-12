--- 
layout:  post 
title:   "One Weird Trick to Untie Landin's Knot"
authors: "Paulette Koronkevich"
date:    2023-10-12 15:00:00
categories: Koronkevich Fall2023
--- 

## Abstract

In this work, we explore Landin’s Knot, which is understood as a pattern for encoding general recursion, including non-termination, that is possible after adding higher-order references to an otherwise terminating language. We observe that this isn’t always true—higher-order references, by themselves, don’t lead to non-termination. The key insight is that Landin’s Knot relies not primarily on references storing functions, but on unrestricted quantification over a function’s environment. We show this through a closure converted language, in which the function’s environment is made explicit and hides the type of the environment through impredicative quantification. Once references are added, this impredicative quantification can be exploited to encode recursion. We conjecture that by restricting the quantification over the environment, higher-order references can be safely added to terminating languages, without resorting to more complex type systems such as linearity, and without restricting references from storing functions.
