This repository contains the source of the **O8** Cosmochrony paper  
*Three-Step Path Fingerprints on LPS Graphs and the Capacity Growth Exponent*.

This work extends the **spectral admissibility sub-programme** by testing the
first fingerprint class that escapes the fixed finite-dimensional obstruction
established in **O6**. Its objective is to determine whether a capacity growth exponent in
the range

$\delta \in [7.4, 10.6]$

can emerge once the admissible state space grows with $q$. In that range the upper bound
$\beta \le 1/(1/2+\delta)$, which O6 proves under an unestablished effective growth hypothesis,
lies inside the phenomenological window $\beta^\*=(0.09,0.13)$; the bound does not select
$\beta^\*$, and $\beta^\*$ is compatible with it only if $\delta<10.611$.

While **O6** proves that no fixed finite-dimensional fingerprint can sustain a
long enough pre-saturation regime, **O7** identifies the correct observable as
the discrete projective capacity $\Sigma_n$ and reformulates the problem as the
search for a regime in which

$\overline{\Sigma}_n \sim p(n)^{-\delta}$.

The present work performs the first explicit construction and test of such a
growing fingerprint.

The central object introduced here is the **three-step permutation-path fingerprint**

$\pi_3(\gamma) = \rho_{\mathrm{perm}}(v_1)\otimes
\rho_{\mathrm{perm}}(v_2)\otimes
\rho_{\mathrm{perm}}(v_3)\in\mathbb{R}^{(q+1)^3},$

where $\rho_{\mathrm{perm}}$ is the permutation representation of
$PSL(2,\mathbb{F}_q)$ on $\mathbb{P}^1(\mathbb{F}_q)$ and
$\gamma=(v_0,v_1,v_2,v_3)$ is a non-backtracking path of length $3$. This gives
an ambient dimension $O(q^3)$ that grows with $q$, thereby escaping the O6
fixed-representation no-go.

# Core Result

The paper establishes a **new obstruction class** to extracting the cascade
exponent on LPS graphs.

Starting from:

- the $k=3$ permutation-path fingerprint
- the O7 capacity observable $\Sigma_n$
- the state-law target $R_n^{(k)}\approx\Phi(\eta_n)$
- numerical experiments on LPS families $X_{p,q}$ for
  $(p,q)\in\{(17,13),(13,17),(5,29),(5,41)\}$

the analysis shows that:

- the fingerprint span continues to grow up to $O(q^2)$ vertices
- the effective pre-saturation window in vertex count is the first one in the
  O-series to grow with $q$
- the O6 algebraic obstruction is genuinely bypassed
- but on LPS graphs this $O(q^2)$-vertex window is compressed to only
  $O(\log q)$ BFS steps by exponential shell growth
- as a consequence, the available fit window is too short to extract a stable
  exponent $\delta$ even though the fingerprint itself is structurally adequate

The observed values

$\delta \in [0.035, 0.177]$

are therefore not interpreted as the true asymptotic exponent, but as the
signature of a geometrically compressed measurement window.

# Structural Role of O8

O8 does not yet derive the phenomenological value of $\delta$.

Instead, it proves that once the O6 fixed-dimensional obstruction is removed,
a deeper limitation appears: **the geometry of the underlying graph family may
itself prevent exponent extraction**.

The logical chain is now:

- **O6**: fixed finite-dimensional fingerprints fail for algebraic reasons
- **O7**: the relevant observable is projective capacity, not raw redundancy
- **O8**: even with a growing fingerprint space, exponential shell growth on
  LPS graphs geometrically compresses the observable window

The failure is therefore no longer attributable to insufficient fingerprint
complexity, but to an intrinsic mismatch between:

- a pre-saturation regime growing in **vertex count**
- and a graph geometry whose BFS shells grow too quickly in **depth**

# What O8 Adds

O8 introduces several decisive new structural results:

- the first explicit **multi-step path fingerprint** with ambient dimension
  $O(q^3)$
- the first explicit fingerprint class that **escapes the O6 no-go**
- the first numerical confirmation of a pre-saturation window growing as
  $O(q^2)$ in vertex count
- the identification of a new obstruction class:
  **geometric compression by exponential shell growth**
- a clear separation between:
    - **algebraic saturation** from fixed-dimensional Hecke dynamics
    - **geometric compression** from expander shell growth
    - the still-open derivation of the true asymptotic exponent $\delta$

# Interpretation of the Obstruction

The obstruction established in O8 has a precise physical and structural meaning
in the Cosmochrony framework.

It shows that the smallness of the effective cascade exponent cannot be read off
from a growing fingerprint space alone. What matters is not only whether the
space of admissible directions expands with $q$, but also whether the graph
geometry provides enough **BFS depth** to observe a genuine power-law regime.

In particular:

- O6 showed that a fixed finite-dimensional space saturates too quickly
- O8 shows that even a growing fingerprint can remain observationally
  insufficient if the graph covers $O(q^2)$ vertices in only $O(\log q)$ steps

Thus the problem is no longer merely one of representation theory. It becomes a
joint problem of:

- admissible state-space growth
- capacity dynamics
- and graph geometry

In this sense, the exponent $\delta$ is not simply a combinatorial property of a
fingerprint, but a dynamical quantity whose observability depends on the depth
structure of the cascade.

# Relation to Previous Steps

O8 preserves all previous structural results:

- spectral admissibility from **Step 1**
- binary-polyhedral maximality from **Step 2**
- three-level ADE stratigraphy from **Step 3**
- projective dynamics and support contraction from **O1**
- hierarchical amplification via growing valence from **O3**
- the open status of a structural bound on the cascade exponent, from **O4** (no bound follows
  from the bounded-flux and Cheeger argument)
- admissible-frontier saturation from **O5**
- fixed finite-dimensional no-go from **O6**
- capacity reformulation and state law from **O7**

It does not modify the mass-hierarchy target itself.
Instead, it shows that the next obstruction lies in the geometry of the graph
family used to probe the growing fingerprint.

# Conceptual Structure

O8 advances the structural chain as follows:

1. Spectral admissibility → mode selection
2. Spectral capacity → binary-polyhedral maximality
3. Spectral stratigraphy → discrete ADE levels
4. O1 → ordering via support contraction
5. O3 → amplification via valence growth
6. O4 → no structural bound on $\beta$ from bounded flux and Cheeger expansion (open)
7. O5 → admissible-frontier saturation and localisation of the problem
8. O6 → no-go theorem for fixed finite-dimensional fingerprints
9. O7 → reformulation in terms of projective capacity
10. O8 → growing path fingerprint and discovery of geometric compression

The programme now excludes not only static finite-dimensional encodings, but
also the LPS expander geometry itself as a suitable setting for direct
measurement of $\delta$ once the observable window is expressed in BFS depth.

# What O8 Resolves

O8 provides:

- a first explicit $k=3$ permutation-path fingerprint in ambient dimension
  $O(q^3)$
- a first numerical confirmation that the effective pre-saturation window grows
  as $O(q^2)$ in vertex count
- a structural demonstration that the O6 obstruction is genuinely overcome
- a proof-of-principle that exponent extraction can still fail for purely
  **geometric** reasons
- a precise localisation of the remaining open problem: one must now change not
  only the fingerprint, but also the graph-growth regime

# Residual Open Problem

What remains open is no longer whether a growing admissible fingerprint can
exist, but how to observe a sufficiently long power-law regime for
$\overline{\Sigma}_n$.

O8 therefore isolates the next necessary step:

a graph family with **sub-exponential shell growth**, so that an
$O(q^2)$-vertex pre-saturation window corresponds to many more than
$O(\log q)$ BFS steps.

The problem is no longer solely:

- build a larger fingerprint

but also:

- provide a geometry in which that fingerprint can unfold over a sufficiently
  long observable cascade.

# Open Directions

1. **Proof of the $O(q^2)$ window scaling**  
   Turn the effective saturation law
   $|S^\*|_{\mathrm{eff}} = O(q^2)$ into a theorem

2. **State-law proof on LPS graphs**  
   Prove that
   $R_n^{(3)} \approx \Phi(\eta_n)$
   holds in the dilute regime with vanishing corrections as $q\to\infty$

3. **Sub-exponential shell-growth graphs**  
   Test the same $k=3$ fingerprint on graph families with polynomial or other
   sub-exponential shell growth, so that the observable window in BFS depth is
   long enough to support exponent extraction

4. **First-principles derivation of $\delta$**  
   Derive the exponent $\delta$ from the spectral and Born--Infeld structure
   directly, without phenomenological input

5. **Beyond the LPS setting**  
   Determine whether the obstruction identified here is specific to expander-like
   shell growth or persists in broader admissible graph families

# Status

This framework is now:

- beyond the fixed finite-dimensional matrix level of **O6**
- expressed in the capacity language introduced by **O7**
- structurally free of the O6 algebraic obstruction
- sharply focused on the geometry-dependent observability of $\delta$

It does not assume:

- phenomenological fitting of the exponent window
- arbitrary large fingerprints without structural interpretation
- that a growing state space alone is sufficient for exponent extraction

# Repository Structure
```
paper/
├── out/      # Compiled O8 PDF
├── tex/      # LaTeX sources
└── README.md
```
# Citation

If you reference this work, please cite:

J. Beau, Three-Step Path Fingerprints on LPS Graphs and the Capacity Growth Exponent, Zenodo, 2026.

# Acknowledgements

Portions of the derivations, conceptual synthesis, and editorial refinement
benefited from iterative interactions with large language models used as
analytical assistants.
All theoretical results and interpretations remain the sole responsibility
of the author.

# Contributions

This repository is intended as a research reference.

Critical feedback, independent verification, and alternative constructions
of growing admissible fingerprints or sub-exponential graph families are
welcome.

Please open an issue to discuss conceptual points,
technical details, or possible extensions.
