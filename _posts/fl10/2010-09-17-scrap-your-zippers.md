--- 
layout:  post 
title:   "Scrap Your Zippers: A Generic Zipper for Heterogeneous Types"
authors: "Michael D. Adams" 
date:    2010-09-17 04:15:00 
categories: Adams Fall2010
--- 

## Abstract

The zipper type provides the ability to efficiently edit tree-shaped
data in a purely functional setting by providing constant time edits
at a focal point in an immutable structure. It is used in a number of
applications and is widely applicable for manipulating tree-shaped
data structures.

The traditional zipper suffer from two major limitations, however.
First, it operates only on homogeneous types. That is to say,
every node the zipper visits must have the same type. In practice,
many tree-shaped types do not satisfy this condition, and thus cannot
be handled by the traditional zipper. Second, the traditional zipper
involves a significant amount of boilerplate code. A custom implementation
must be written for each type the zipper traverses.
This is error prone and must be updated whenever the type being
traversed changes.

The generic zipper presented in this talk overcomes these
limitations. It operates over any type and requires no boilerplate
code to be written by the user. The only restriction is that the types
traversed must be instances of the Data class from the Scrap your
Boilerplate framework.

