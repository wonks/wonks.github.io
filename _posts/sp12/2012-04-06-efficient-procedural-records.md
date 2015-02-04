--- 
layout:  post 
title:   "Efficient Procedural Records"
authors: "Andrew Keep" 
date:    2012-04-06 04:15:00 
categories: Keep Spring2012
--- 
## Abstract

Many languages include a syntax for declaring programmer-defined structured
data types, i.e., structs or records.  At a minimum, the syntax defines the
record's name and a set of named fields.  Because it is defined syntactically,
the compiler can open-code allocation operations and compile field references
and assignments into single memory references, with field offsets calculated at
compile time.  R6RS supports syntactic record definitions but also allows
records to be defined procedurally, i.e., via a set of run-time operations.
Indeed, the procedural interface is considered to be the primitive interface,
and the syntactic interface is designed to be macro expandable into code that
uses the procedural interface.

The procedural layer allows arbitrary new record types to be created at run
time, facilitating the creation of portable interpreters that interoperate with
compiled code.  It also supports the creation of portable printers and
debuggers, which can obtain an RTD from a record instance and use it to access
or even modify the fields of the instance.  This added flexibility comes at a
potentially substantial cost, since the information required to open-code
allocation, field reference, and field assignment operations is not generally
available until run time.  In many cases, however, such as when the record
operators are produced by the syntactic interface, the information can be
determined statically, enabling the generation of efficient code.  In this
talk, I (briefly) describe the syntactic, procedural, and inspection layers of
the record system and then describe how Chez Scheme utilizes cp0 to generate
efficient record code.

