--- 
layout:  post 
title:   "Hygienic Literate Programming: Lessons from ChezWEB"
authors: "Aaron Hsu" 
date:    2011-10-14 04:15:00 
categories: Hsu Fall2011
--- 
## Abstract

Literate programming systems are a class of domain specific languages
designed to encourage writing programs specifically to be read as
essays or books by humans instead of by machines.  Systems like CWEB,
WEB, and ChezWEB allow the user to associate arbitrary code bodies
with a concise but natural language description.  That description may
then be referred to in other sections of the program source, and the
code body associated with the description is substituted for the
reference in the program source.  ChezWEB implements code reordering
according to a specific set of "hygienic" principles. This talk
describes what these principles are and why they make sense for
literate programming. Additionally, I will explore the implementation
of these principles in the syntax-case system through a series of
macros designed to test and strengthen your understanding of macros
and hygiene; bring your macro hats!

