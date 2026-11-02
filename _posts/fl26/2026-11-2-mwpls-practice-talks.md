---
layout:  post
title:   "Midwest PL Summit (MWPLS) Practice Talks"
authors: "Ethan Hawk, Yafei Yang, Yuquan Fu, and Kelton OBrien"
date:    2026-11-2 15:00:00
categories: MWPLS Fall2026
usemathjax: true
---

[The ninth Midwest Programming Languages Summit
(MWPLS'26)](https://2026.mwpls.org/) will take place on Friday, November 6,
2026, hosted by the University of Iowa.

## Time and Location

* **Date:** Monday, November 2
* **Time:** 3:00 PM
* **Location:** Luddy Hall (BLIF) 3069

## Talks

* **Incremental Hygienic Macros via Demand-Driven Computation** — Ethan Hawk

  > Modern compilers are incremental, but when programmers use macros, most
  > incremental compilers give up and recompile the macros and downstream uses
  > from scratch. We show that hygenic macro expansion can be expressed using
  > demand-driven incremental computation, and thus particpate fully in
  > incremental compilation. Traditional implementations of hygiene resist
  > incrementalization, yet we show that they can be refactored to support
  > reuse despite a wide variety of code changes.
  >
  > We combine several techniques to enable incremental macro expansion. Stable
  > pedigrees give each generated scope and local binding a consistent address
  > based on where it is created during expansion. Shared tables are
  > partitioned into individually tracked entries, so updating one binding does
  > not invalidate unrelated lookups. The system delays propagating hygiene
  > information through nested syntax until that syntax is inspected, and
  > treats source positions as dependencies only for macros that observe them.
  > Finally, the expander avoids recording the same dependencies repeatedly
  > across nested expansion steps. On re-expansion, a cached step is reused if
  > everything previously depended upon is unchanged; otherwise the step runs
  > again.
  >
  > We apply these techniques to reduced version of Racket's macro expander
  > atop a port of the Adapton incremental computation design to Racket and
  > confirm that the resulting system produces from-scratch consistent results
  > in all tests. Our experiments show substantial reductions in repeated
  > expansion work for both unchanged inputs and local edits, with
  > recomputation following the affected portion of the expansion. These
  > results establish that the complexities of modern hygenic macro systems do
  > not preclude precise incremental reuse.

* **Formalizing einsum with Named Tensor Notation** — Yafei Yang

  > Einstein notation (einsum) is a widely adopted tensor operation that has
  > proven useful in areas such as machine learning and quantum computing. But
  > it had no formal semantics until recently, and its properties had no
  > mechanized verification. We formalize the denotational semantics of a
  > language of tensors (multi-dimensional arrays) that supports einsum and
  > repeated tensors (expand). With this semantics, we verify equational
  > rewriting rules about einsum and expand that improve the performance of
  > tensor computation. Whereas typical languages use unnamed tensors, whose
  > shape is a sequence of natural numbers, we found it advantageous for
  > mechanization to use named tensors, whose shape is a finite map from names
  > to natural numbers. To our knowledge, this is the first time that the
  > semantics and rewriting rules of einsum are mechanized in a proof
  > assistant. Our solution is agnostic to proof assistants; we have
  > implemented it in Lean and partially in Agda.

* **Revisiting Occurrence Typing, Semantically** — Yuquan Fu, Carlo Angiuli, and Sam Tobin-Hochstadt

  > Over the past two decades, numerous systems have brought some of the
  > benefits of dependent typing to a wide variety of new programming
  > languages, often by restricting which terms can appear inside types. Such
  > techniques are known as refinement types, occurrence typing, liquid types,
  > and path dependent types, among others. However, the restrictions adopted
  > by these systems often break the substitution property, because they
  > explicitly disallow the ability to substitute arbitrary terms for variables
  > inside types. This leads to significant complexity in the design and
  > metatheory of these systems, increasing the possibility of significant
  > errors.
  >
  > We consider a specific line of work on occurrence typing, namely, the
  > calculus underlying Typed Racket due to Tobin-Hochstadt and
  > Felleisen(2010). We show that the fundamental challenge of substitution
  > into types resulted in multiple flaws in the formalism and the syntactic
  > type soundness theorem of this work. These flaws are replicated in several
  > other papers building on this work, and also surface as a soundness bug in
  > Typed Racket itself. We identify and repair these problems, revising the
  > core calculus of Typed Racket and giving a semantic type soundness proof
  > using step-indexed logical relations, formalized in Lean. We argue that
  > this approach is simpler than it may seem, and easily scales to handle the
  > complexity of the occurrence typing in Typed Racket.

* **A Dependent Type Theory with Strictly Associative and Unital Sigma Types** — Kelton OBrien

  > We present "Cormorant", a version of Martin-Löf Dependent Type Theory (MLTT)
  > with a $$\Sigma$$ type that is judgmentally associative and unital. That is,
  > Cormorant affirms judgemental equalities $$\Gamma \vdash \Sigma(\Sigma A B)
  > C \equiv \Sigma A (\Sigma B C)$$ and $$\Gamma \vdash \Sigma A \mathsf{Unit}
  > \equiv A$$, as well as the required context equations for these equalities
  > to be well formed. These equalities we now enjoy make pose some difficulties
  > in constructing a typechecker for the theory, but we present some techniques
  > we use to do so. We present the theory, as well as algorithmic elaborator
  > from a surface syntax into the logic, and demonstrate our implementation of
  > the elaborator by showing some novel programs that are possible to write in
  > our theory that are not possible to write in MLTT. We also describe the
  > currently-in-progress work on proving important metatheorems (chiefly
  > normalization), which Cormorant appears to enjoy despite the fact that it
  > does not have injective type constructors.
