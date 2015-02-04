--- 
layout:  post 
title:   "A Meta-Scheduler for the Par-Monad: Composable Scheduling for the Heterogeneous Cloud"
authors: "Adam Foltzer" 
date:    2012-04-20 04:15:00 
categories: Foltzer Spring2012
--- 
## Abstract

Modern parallel computing hardware demands increasingly specialized
attention to the details of scheduling and load balancing across
heterogeneous execution resources that may include GPU and cloud
environments, in addition to traditional CPUs. Many existing solutions
address the challenges of particular resources, but do so in
isolation, and in general do not compose within larger systems. We
propose a general, composable abstraction for execution resources,
along with a continuation-based meta-scheduler that harnesses those
resources in the context of a deterministic parallel programming
library for Haskell. We demonstrate performance benefits of combined
CPU/GPU scheduling over either alone, and of combined
multithreaded/distributed scheduling over existing distributed
programming approaches for Haskell.

This will be a short talk (~20 minutes) to practice for a possible
future presentation in a conference venue. As such, I'd very much
appreciate feedback on presentation style and delivery in addition to
comments on the substance of the work.  This is joint work with
Abhishek Kulkarni, Rebecca Swords, Sajith Sasidharan, Eric Jiang, and
Ryan R. Newton.

