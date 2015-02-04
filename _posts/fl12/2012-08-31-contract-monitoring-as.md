--- 
layout:  post 
title:   "Contract Monitoring as an Effect"
authors: "Zack Owens" 
date:    2012-08-31 04:15:00 
categories: Owens Fall2012
--- 
## Abstract

Contracts are a tool used by software engineers to validate assumptions
made during the development of software systems. In the world of
higher-order programming, higher-order contracts serve as a
compositional mechanism to ensure that each function application
satisfies the argument and result predicates that form a higher-order
contract. The usual implementation of contract systems include a
contract monitoring component in the runtime. Most formal incarnations
of contracts treat the monitor as a transparent component with only one
benign effect: terminating programs that violate their contracts. The
monitoring of contracts is, however, far from being this benign: it may
completely changed what part of the program gets evaluated and in what
order. Such effects were noticed earlier in the context of lazy
languages but their full impact has not been fully appreciated. In the
talk, contract properties will be framed in a new context in which the
monitoring of contracts is viewed as an explicit effect.

