--- 
layout:  post 
title:   "Dynamic Inference of Static Types for Ruby"
authors: "James T. Perconti" 
date:    2011-02-11 04:15:00 
categories: Perconti Spring2011
--- 
## Abstract

This talk presents a POPL 2011 paper of the same name by 
Johg-hoon (David) An, Avik Chaudhuri, Jeffrey S. Foster, and Michael 
Hicks.  The paper can be found at 
http://www.cs.umd.edu/~avik/projects/distr/. It 
introduces "constraint-based dynamic type inference, a technique that 
infers static types based on dynamic program executions."  The authors 
develop and formalize an algorithm to generate constraints on fields and 
method arguments as they are used at runtime, which can be solved to infer 
types for these entities.  They are also able to show a soundness result: 
"if training runs cover all syntactic paths through each method of a 
class, then the inferred type for that class is sound."  Finally, they 
discuss their implementation of the algorithm, called Rubydust.

