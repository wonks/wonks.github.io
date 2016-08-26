--- 
layout:  post 
title:   "Expressing Contract Monitoring Strategies for Call-by-Value and Call-by-Name Calculi"
authors: "Cameron Swords"
date:    2016-04-15 04:15:00 
categories: Swords Spring2016
--- 

## Abstract

Software Contracts and contract monitoring have gained significant popularity in
dynamically-typed functional programming languages in recent years. This
popularity has also given rise to myriad monitoring
strategies---characterizations of how these contracts interact with the
underlying user evaluator, and how these interactions impact program behavior.

In this whiteboard talk, I will motivate and present our system for describing
these strategies and their interactions in a single, core framework that
leverages process communication primitives to model contract monitoring as
evaluator interactions.  I will also talk about my current work of reformulating
the system for a call-by-name semantics.

If time allows, I will also sketch future work: exploration of the design space
of contract monitoring, implementation details, and contracts in the presence of
other effects.
