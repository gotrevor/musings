---
title: Small results
status: growing
started: 2026-10-06
reviewed-by-trevor: pending
key-claims:
  - Each linked note is the authority for its result.  It says what is proved, what is assumed, and what is not claimed.  The one-liners here are pointers, not statements.
claims:
  - Most results are checked in Lean.  Some are conditional on cited published theorems, and the note says which.
  - Each result is new as far as we could find, within the limits of the prior-work search the note records.
---

# Small results 🧮

[ Written by Claude at Trevor's direction. ]

🌿 *A running list, newest first.  Comments and corrections welcome in [Discussions](https://github.com/gotrevor/musings/discussions).*

These came out of the Lean work: new results, but small ones, not big enough to write to anyone about.  Each has a one-page write-up in its repo that states the result, links the Lean declarations, names any cited theorem it assumes, and says what is not claimed.  Read the write-up, not the one-liner.

## New mathematics

### 2026-10-06

- **[P(7,5,6) holds at 26 points](https://github.com/gotrevor/es7-ladder/blob/master/docs/notes/p756.md).**  Every 26 points in general position contain a convex 7-gon, a 5-cap or a 6-cup.  This is the lowest open rung of the Erdős–Tuza–Valtr ladder toward ES(7) = 33.  A SAT computation, not a Lean proof.
- **[Cantor-set points with any irrationality exponent, normal to every base prime to 3](https://github.com/gotrevor/normal-numbers/blob/wip/g5-prime-subset/docs/notes/cantor-exact-exponent-normal.md).**  For every rational μ₀ > 2, a computable point of the middle-third Cantor set has irrationality exponent exactly μ₀ and is normal to every base b with 3 ∤ b.
- **[Keeping ξ(3/2)ⁿ far from the integers: 0.1228](https://github.com/gotrevor/collatz-moonshot/blob/ren/g2-hunt-flatto-ceiling/docs/notes/far-from-integers-0-1228.md).**  Some ξ keeps every ξ(3/2)ⁿ at distance at least 307/2500 from the integers, up from 5/48 ≈ 0.1042 (Dubickas 2008).  Memoryless constructions of this kind cannot pass 7/57.
- **[How short an arc can hold an orbit of ξ(3/2)ⁿ: the 2/3 edge](https://github.com/gotrevor/collatz-moonshot/blob/ren/g2-hunt-flatto-ceiling/docs/notes/arc-traps-two-thirds-edge.md).**  Mahler's 3/2 question, restricted to constructions that read finitely many low bits: no such construction keeps the orbit in an arc shorter than 2/3.

### 2026-10-05

- **[Shifted Mills constants are transcendental](https://github.com/gotrevor/lean-formalizations/blob/main/docs/notes/shifted-mills-transcendence.md).**  For every integer s ≠ 0, the least A > 1 with ⌊A^(3^k + s)⌋ prime for all k is transcendental.  Mills' constant itself (s = 0) is not covered.
- **[Practical numbers: three small observations](https://github.com/gotrevor/lean-formalizations/blob/main/docs/notes/practical-numbers.md).**  The first: plugging Tao–Trudgian–Yang's new exponent pair into Weingartner's theorem puts practical numbers in intervals [x − x^β, x] for β > 0.486987….

### 2026-10-04

- **[Pulari's two questions on naming maps](https://github.com/gotrevor/normal-numbers/blob/wip/g5-prime-subset/docs/notes/pulari-pushdown-naming-maps.md).**  Yes to the deterministic-pushdown question, for every base k ≥ 7 (k ≥ 3 with one believed lemma).  And non-invertible synchronous relabelings cannot break the equidistribution characterization.  Conditional on cited results.

### 2026-10-03

- **[Bugeaud Problem 10.36: one ξ, badly approximable to every base](https://github.com/gotrevor/normal-numbers/blob/wip/g5-prime-subset/docs/notes/bugeaud-10-36-uniform-bad.md).**  There is ξ with ‖bⁿξ‖ > b^(−24) for every base b ≥ 2 and every n ≥ 0.  Unconditional.
- **[Bugeaud Problem 10.37: a Liouville number in the Cantor set, normal to base 2](https://github.com/gotrevor/normal-numbers/blob/wip/g5-prime-subset/docs/notes/bugeaud-10-37-cantor-liouville.md).**  A computable one.
- **[Bergelson–Downarowicz's questions on deterministic numbers](https://github.com/gotrevor/normal-numbers/blob/wip/g5-prime-subset/docs/notes/deterministic-numbers.md).**  No to both.  Products, ratios and reciprocal products of two deterministic numbers form a set of Hausdorff dimension 0 (unconditional), and a reciprocal of a deterministic number can fail to be deterministic (conditional).
- **[Two explicit normal numbers](https://github.com/gotrevor/normal-numbers/blob/wip/g5-prime-subset/docs/notes/explicit-normal-bad-and-reciprocal.md).**  An absolutely normal number whose partial quotients are all 1 or 2, and an absolutely normal number whose reciprocal is not normal.  Conditional on cited Fourier-decay theorems.
- **[Normal in base 2 and every odd base, with fast base-2 discrepancy](https://github.com/gotrevor/normal-numbers/blob/wip/g5-prime-subset/docs/notes/odd-bases-fast-base-2-discrepancy.md).**  Base-2 discrepancy O((log N)²/N).  Conditional on cited results.

### 2026-10-02

- **[Erdős Problem #257: new cases](https://github.com/gotrevor/normal-numbers/blob/wip/g5-prime-subset/docs/notes/erdos-257.md).**  For k ≥ 2 and S a set of primes with a Mertens rate, Σ_{n∈k·S} 1/(2ⁿ − 1) is irrational, and in fact its base-2^k expansion contains every finite word.
- **[Manai's questions on normality under polynomials](https://github.com/gotrevor/normal-numbers/blob/wip/g5-prime-subset/docs/notes/computable-normal-square-not-normal.md).**  For every k ≥ 2, a computable x with p(x) normal for every integer polynomial of degree 1 to k − 1, while x^k is not normal.  Conditional on Baker–Banaji's decay theorem.

## Formalizations of known results

Lean formalizations of results that were already proved but not yet formalized.  The lists live in the repos:

- 🖼️ [lean-gallery](https://github.com/gotrevor/lean-gallery#contents): the finished, curated ones (Goodstein, Kirby–Paris hydra, several Erdős problems).
- 📚 [lean-formalizations](https://github.com/gotrevor/lean-formalizations#contents): the wider set (Mills, Curtis's Frobenius no-formula theorem, Euler's power tower, Wantzel, Hermite–Lindemann, and more).
- 🌀 [tao-collatz](https://github.com/gotrevor/tao-collatz): Tao 2019, almost all Collatz orbits attain almost bounded values.
- 🏛️ [goodstein-independence](https://github.com/FormalizedFormalLogic/goodstein-independence): PA does not prove Goodstein's theorem (Kirby–Paris), in the FormalizedFormalLogic org.

---

*About this page: compiled by Claude (Ren, Trevor's Claude Code assistant) at Trevor's direction from the write-ups it links.  The one-liners are Claude's summaries; the write-ups and their Lean files are the authority.*
