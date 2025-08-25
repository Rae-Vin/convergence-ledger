# Law of Recursion (LoR) --- Formal Statement

## 0) Plain statement (one line)

**Recursive generation produces higher-order structures that (i)
preserve lower-order invariants and (ii) induce new effective laws at
coarser descriptions,** provided those structures satisfy the **Law of
Stability** (LoS).

------------------------------------------------------------------------

## 1) Core objects & notation

-   **System** (S): a set of admissible configurations (X subset of
    space).
-   **Constraints / invariants** (C = {I_j}): conservation or legality
    rules (e.g., mass/energy/charge; codon legality).
-   **Recursive generator** (R: X→X): a transformation producing new
    configurations from previous ones (iteration, recursion,
    composition).
-   **Coarse-graining / projection** (G_k: X→Y_k): level-k description
    (e.g., words→sentences; particles→fields).
-   **Effective law at level k**: L_k s.t. G_k ∘ R ≈ L_k ∘ G_k (up to
    error ε_k).
-   **Stability functional** (V: X→R≥0) (from LoS): decreases or remains
    bounded along persistent trajectories.
-   **Scale ladder**: L_0 (micro) → L_1 (meso) → L_2 (macro) ... with
    projections G_1, G_2, ...

------------------------------------------------------------------------

## 2) The Law (formal)

**Law of Recursion.**\
Let (S, R, C) be a recursive system with invariants C. Suppose there
exists a stability functional V (LoS). Then:

1.  (Preservation) Each iteration preserves invariants: I_j(R(x)) =
    I_j(x).\
2.  (Induction) There exists a sequence of coarse laws {L_k} such that
    for each k,\
    G_k ∘ R\^n ≈ L_k\^n ∘ G_k (uniformly for bounded n).\
3.  (Emergence) Novel invariants J_k appear at higher levels, stable
    under L_k.\
4.  (Universality) Different micro-generators {R} sharing C but
    differing in details converge to the same {L_k}, provided stability
    holds.

------------------------------------------------------------------------

## 3) Interpretation across domains

-   **Physics:** Iterating local rules (quantum fields, cellular
    automata) under LoS produces conservation laws at larger scales
    (thermodynamics, relativity symmetries).\
-   **Linguistics / RSBS:** Recursive symbolic expansions under
    stability yield grammar laws, semantic coherence, eventually
    language-like emergent laws.\
-   **Cognition / AGI:** Self-recursive symbol manipulation under LoS
    stabilizes and yields effective meta-laws (reasoning, planning).\
-   **Mathematics:** Recursive definitions (e.g., recurrence relations)
    always imply closed forms or asymptotics that behave like new
    "laws."

------------------------------------------------------------------------

## 4) Relation to Law of Stability (LoS)

-   LoS ensures *boundedness* (no blow-up).\
-   LoR ensures *lawfulness* (each recursion induces effective laws).\
-   Together: RSBS + Braid imply LoS+LoR ⇒ symbolic universes that are
    both stable and lawful.

------------------------------------------------------------------------

## 5) Consequence (AGI + physics + math)

The LoR suggests that any recursive symbolic generator---if
stable---necessarily bootstraps new effective laws. This explains why
RSBS produced grammar-like behaviors so quickly: the LoR guarantees
*law-induction* is a mathematical necessity, not a heuristic.\
It also bridges math/physics: renormalization, effective field theory,
grammar emergence, and AI scaling are all corollaries.

------------------------------------------------------------------------

## 6) Plain restatement (closing)

**If recursion is stable, laws emerge.**\
That is the Law of Recursion.
