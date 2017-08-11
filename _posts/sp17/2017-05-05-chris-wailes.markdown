--- 
layout:  post 
title:   "Evaluation of Network/Performance Models for Topologically-Aware Load Balancing: I've Never Meta-Metric I Didn't Like"
authors: "Chris Wailes" 
date:    2017-05-05 04:15:00 
categories: Wailes Spring2017
--- 

## Abstract

The hypothesis driving research into topologically-aware load balancing (TALB) is that the way data travels over a network impacts the total runtime of parallel applications.  To test this hypothesis we need to build network/performance models and analyze the strength of their correlation to observed experimental values.  Unfortunately, previous work has failed to sufficiently isolate the model being evaluated from the mathematical optimization techniques and load-balancing mechanisms of the runtime environment.  In this talk I will present a new approach to evaluating network/performance models in the context of TALB.
