--- 
layout:  post 
title:   "Pycket Using Racket Bytecode"
authors: "Caner Derici"
date:    2016-04-22 04:15:00 
categories: Derici Pycket Spring2016
--- 

## Abstract

Pycket is an experimental JIT compiler that implements Racket,
developed using the RPython translation framework. It expands the
given Racket code using Racket's own macro expander, and transforms
the fully expanded code into Pycket AST. Our idea is to obtain this
AST using Racket bytecode instead of the expanded surface code, and
see if Pycket can benefit from various optimizations performed by the
Racket bytecode compiler.

The talk will be in three parts. First we'll look into the Racket
bytecode, and talk a bit about the bytecode compiler. Second we'll
talk about transforming Racket bytecode into Pycket AST. Finally we'll
talk a bit about optimizations happening in the Racket compiler and
see some recent performance results of Pycket using the bytecode
expansion.
