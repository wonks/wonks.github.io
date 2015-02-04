--- 
layout:  post 
title:   "Code Contracts in a World of Uncertainty"
authors: "Michael Hansen" 
date:    2011-04-08 04:15:00 
categories: Hansen Spring2011
--- 
## Abstract

I've been working with Amr Sabry and Amal Ahmed to develop a contract system
where some contracts may probabilistically succeed with "incorrect" values. This
is done both for performance reasons and for certain domains where a
deterministic check is infeasible. An analogy with database-query dependency
checking is made for blame assignment, where contract labels in our system take
on the role of data colors. This work is very preliminary, so feedback will be
appreciated.

