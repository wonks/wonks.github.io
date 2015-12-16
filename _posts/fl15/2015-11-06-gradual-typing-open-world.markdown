--- 
layout:  post 
title:   "Gradual Typing in an Open World"
authors: "Michael Vitousek" 
date:    2015-11-06 04:15:00 
categories: Vitousek GradualTyping Fall2015
--- 
## Abstract

Gradual typing combines static and dynamic typing
in the same language, offering the benefits of both to
programmers. Static typing provides error detection and strong
guarantees while dynamic typing enables rapid prototyping and
flexible programming idioms. For programmers to fully take advantage
of a gradual type system, however, they must be able to trust their
type annotations, and so runtime checks must be performed at the
boundaries of static and dynamic code to ensure that static types
are respected. Higher order and mutable values cannot be completely
checked at these boundaries, and so additional checks must be
performed at their use sites. Traditionally, this has been achieved
by installing wrappers or proxies on such values that moderate the
flow of data between static and dynamic, but these can cause
problems if the language supports comparison of object identity 
or has a foreign function interface.

Reticulated Python is a gradually typed variant of Python
implemented via a source-to-source translator for Python 3. It
implements a proxy-free alternative design named transient casts.
I'll discuss the design and semantics of transient casts and 
shows that not only are they sound, but they work in an
open-world setting in which the Reticulated translator has only been
applied to some of the program; the rest is untranslated Python. I'll
formalize this "open world soundness" property and discuss how we proved
that it holds for a calculus modelling Reticulated. 
