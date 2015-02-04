--- 
layout:  post 
title:   "Ftypes: structured foreign data access"
authors: "Andrew Keep" 
date:    2011-04-22 04:15:00 
categories: Keep Spring2011
--- 
## Abstract

Foreign function interfaces are an important feature of many modern languages
allowing programmers to interface with libraries (especially system libraries)
not otherwise available in the programming language. Chez Scheme has long
supported an interface for defining foreign procedures, accessing foreign data,
and defining Scheme procedures that can be called by foreign functions. This
interface provides easy access to basic C data types and procedures that make
use of them, but is more difficult to use for structured data commonly used in C
functions. The foreign-type or ftype system, provides a flexible way for
accessing and mutating structured data, including support for C's structs,
unions, and bit fields. Ftypes can be used when defining foreign procedures and
Scheme procedures callable from C, making it easier to interface with C
functions that make use of these features. In this talk I will demonstrate the
new ftype functionality and describe its implementation.

