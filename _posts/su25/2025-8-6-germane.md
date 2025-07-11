---
layout:  post
title:   "Analyzing Control Flow More Like a Human"
authors: "Kimball Germane"
date:    2025-8-6 13:00:00
categories: Germane Summer2025
---

## Time and Location

* **Date:** Wednesday, August 6
* **Time:** 1:00-2:00PM
* **Location:** Luddy Hall 1104 (tentative)

## Abstract

Control-flow analysis has been around for over four decades. Over this time
period, the typical formulation has remained essentially an exhaustive analysis
over whole programs---an analyzer ingests an entire higher-order program and
produces a flow fact for each point therein. An alternative approach is
*demand-driven*. Implementing this approach, an analyzer allows the user to
indicate a point within a higher-order program and subsequently determines its
flow fact, determining as few subsidiary facts as possible. The analyzer keeps
the set of subsidiary facts relatively small by exploring control flow both
forwards and backwards, similar to how a human might reason. This talk
introduces the demand-driven approach, discusses aspects that make it
particularly appealing for today's language infrastructure and tooling, and
outlines possible applications and enhancements.
