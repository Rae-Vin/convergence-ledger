# Law of Entropy (LoE) — Formal Statement

## 0) Plain statement (one line)

**Every recursive system evolves within an entropic gradient.**  
In a closed description, effective entropy is non-decreasing; any persistent decrease in entropy (order maintenance or growth) requires **work, compression, or stabilization** supplied by the system or its environment. Entropy thus sets the **cost** and **limit** against which **Recursion (LoR)** generates structure and **Stability (LoS)** selects/compresses it.

---

## 1) Core objects & notation (aligned to LoR/LoS)

- **System** \( \mathcal{S} = (X,\mathcal{C},R) \): admissible state space \(X\), invariants/constraints \( \mathcal{C}=\{I_j\} \), recursive generator \( R:X\to X \) (or family \( \{R_t\} \)).
- **State process** \( \{x_t\}_{t\ge 0} \), distribution \( \mu_t \) on \(X\).
- **Stability functional** \( V:X\to \mathbb{R}_{\ge 0} \) (from LoS), Lyapunov-like.
- **Coarse-graining** \( G_k: X\to Y_k\), effective law \( L_k \) s.t. \( G_k\circ R \approx L_k\circ G_k\) (LoR).
- **Entropy measures**
  - **Shannon**: \( H(\mu) = -\sum_x \mu(x)\log\mu(x) \) (or differential).
  - **Algorithmic/MDL length**: \( L_{\text{MDL}}(x_{1:T}) \) (description length).
  - **Entropy rate**: \( h = \lim_{T\to\infty}\frac{1}{T} H(X_{1:T}) \).
  - **Entropy production** (stochastic thermodynamics proxy):  
    \( \sigma_{t} \;\approx\; D_{\mathrm{KL}}\!\left(p(x_{t+1}\mid x_t)\, \middle\|\, p^\dagger(x_t\mid x_{t+1})\right) \;\ge 0 \).
- **Free energy–like objective** (variational analogy):  
  \( \mathcal{F}[q] \;=\; \mathbb{E}_{q}\![E(x)] \;-\; T\, S[q] \), with \(S[q]\) an entropy functional (Shannon/MDL) and \(E\) a task/energy proxy (loss).

---

## 2) Axioms of the Law of Entropy (LoE.1–LoE.8)

**LoE.1 (Second-law monotonicity, closed description).**  
For a closed description of the system (no external work/compression), the **effective entropy** does not decrease on average:
\[
\Delta H_{\text{eff}} \;\equiv\; H(\mu_{t+1}) - H(\mu_{t}) \;\ge\; 0
\qquad\text{and/or}\qquad \sigma_t \;\ge\; 0.
\]

**LoE.2 (Work–information inequality / Landauer bound).**  
To **erase** \( \Delta I \) bits of uncertainty, the system must pay a cost:
\[
W \;\ge\; k_B\,T\,(\ln 2)\,\Delta I .
\]

**LoE.3 (Compression–entropy equivalence, MDL).**  
\[
H_{\text{eff}}(X_{1:T}) \;\le\; L_{\text{MDL}}(X_{1:T}) \;+\; \mathcal{O}(1).
\]

**LoE.4 (Coarse-graining inequality / DPI).**  
\[
I(Y;Z) \;\le\; I(X;Z).
\]

**LoE.5 (Entropy–stability tradeoff).**  
\[
\dot{H}_{\text{eff}} \;-\; \alpha\,(-\dot{V}) \;\le\; \beta.
\]

**LoE.6 (Entropy budget across scales).**  
\[
H_{k+1} \;\le\; H_{k} \;-\; \Delta I_{k\to k+1} \;+\; \varepsilon_k .
\]

**LoE.7 (Open systems & entropy flow).**  
\[
\Delta H_{\text{sys}} \;+\; \Delta H_{\text{env}} \;=\; \sigma_{\text{tot}} \;\ge\; 0 .
\]

**LoE.8 (Noise floor / resolution bound).**  
Any representation has a floor \( \eta > 0 \).

---

## 3) Coupling LoE with LoR & LoS

- **LoR (Generator):** Recursion *creates* higher-order patterns.  
- **LoS (Selector):** Stability *selects* coherent patterns.  
- **LoE (Limiter):** Entropy *prices* and *limits* them.

Persistence score:  
\[
\text{Persistence}(t) \;\propto\; \frac{-\,\dot{V}(t)}{\dot{H}_{\text{eff}}(t)+\varepsilon}.
\]

---

## 4) Operationalization

- **RSBS:** Token entropy, perplexity, MI across turns, MDL compression, entropy production proxy.  
- **VUS:** Conservation drift, PDE fit error, coarse entropy, entropy flow.

---

## 5) Falsification protocols

E1–E6 as outlined (closed monotonicity, work–bits, MDL compression, scale budget, critic off/on, noise floor).

---

## 6) Triad summary

- **LoR (Recursion)**: *Generates* laws.  
- **LoS (Stability)**: *Preserves* coherence.  
- **LoE (Entropy)**: *Limits/prices* order.

**If recursion is stable, laws emerge (LoR+LoS). To keep them, you must pay entropy’s price (LoE).**
