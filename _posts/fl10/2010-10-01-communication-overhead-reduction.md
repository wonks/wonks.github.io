--- 
layout:  post 
title:   "Communication overhead reduction using static analysis"
authors: "Nilesh Mahajan" 
date:    2010-10-01 04:15:00 
categories: Mahajan Fall2010
--- 

Video: http://blip.tv/file/4196565 or http://www.sacrideo.us/~arcfide/vid/pl_wonks/nilesh_20101001.html (WEBM HTML5 capable browser required)

## Abstract

Communication related optimizations form an interesting class of
compiler optimizations. Data-flow analysis can be used to determine
efficient placement of communication primitives (e.g. send, receive).
In this talk we will see how data flow equations can be set up to
perform various optimizations like communication-computation overlap,
message coalescing, vector message pipelining. I will start with a
brief introduction to data-flow analysis, proceed to explain the
data-flow equations required for the optimizations. I will also talk
about different approaches to verify these analyses. Finally I would
like to discuss the efficacy of these optimizations and whether
similar analyses can be applied to memory hierarchy.

