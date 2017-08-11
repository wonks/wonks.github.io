--- 
layout:  post 
title:   "Automatically generating clojure.spec annotations"
authors: "Ambrose Bonnaire-Sergeant" 
date:    2017-04-10 04:15:00 
categories: Bonnaire-Sergeant Spring2017
--- 

## Abstract

The initial burden of gradually typing a dynamic program
is often manually reverse engineering and writing annotations.

This talk will give an overview of a tool we have developed
that, given a set of unit tests for a Clojure program, can generate an
appropriate set of clojure.spec and core.typed annotations that can
help fully or partially check a program.
