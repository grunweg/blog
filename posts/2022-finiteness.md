---
author: 'Kyle Miller'
category: 'New in mathlib'
date: 2022-06-13 12:00:00 UTC+01:00
description: ''
has_math: true
link: ''
slug: finite-types
tags: ''
title: Finiteness in mathlib
type: text
---

If you've ever worked with finite types and sets in mathlib, then you're sure to be familiar with the struggle to get the right `decidable` instances,
the debate about whether it is a good idea or not to use `open_locale classical`, or the decision for whether to use `noncomputable` definitions and `fintype` instances
(and whether to put `noncomputable theory` at the top of your file).
Learning these features of Lean seems to be an art in itself, and sometimes it seems that the best strategy is to leave these struggles to the decidability experts
on the Lean Zulip, where they can figure out, for example, what would be the most general `decidable` and `fintype` instances for a `simp` lemma.
An ongoing project in mathlib is to restructure how we handle finiteness so that none of these are issues for the common case of formalizing classical mathematics.

<!-- TEASER_END -->

# What does it mean to be finite?



notes:
* risk in having duplication
* computability vs constructiveness (vs classical)
* `fintype` for computation, `finite` for mere fact
* future: will have `finite_set` for a `set` that satisfies `set.finite` (`set_like`)
* 
