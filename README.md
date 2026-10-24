# Fibrewise Born-Infeld Capacity Lapse and Gravitational Time Dilation (LC-O2)

This repository contains the source of the paper
*Fibrewise Born-Infeld Capacity Lapse and Gravitational Time Dilation
(LC-O2 of the Lorentz Capacity Programme)*
(`Beau2026lco2`).

## Overview

The paper **TempProj** (`Beau2026tp`) constructs the temporal residual map
$\mathcal{P}_\tau^{\mathrm{Q5b}}$ in the homogeneous (flat-space) regime and proves uniqueness.
The present paper (LC-O2) extends this construction to **non-homogeneous fibrewise regimes**,
where a localised spectral occupancy $\epsilon(x)$ reduces the local BI capacity budget.

## Main Result

In a non-homogeneous configuration, the local BI capacity radius is
$R(x)^2 = 1 - \epsilon(x)$.
The fibrewise temporal residual map factorises canonically as:

$$\mathcal{P}_{\tau,x}^{\mathrm{Q5b}}\,\Sigma^{\mathrm{tot}}(x,n)
= R(x)\,\sqrt{f(x,n)\bigl(2 - f(x,n)\bigr)}$$

where $f(x,n) = 1 - \beta(x,n)$ and $\beta(x,n)$ is the local normalised spatial mobility.

The temporal residual capacity per ordering step at $x$ is

$$|F^\tau(x,n)| = \frac{R(x)}{\gamma},$$

a capacity increment, distinct from the constant ordering step $d\tau/dn = \Delta\tau$. **Gravitational time
dilation** is its reading as the proper-time rate $d\tau_u/d\hat\tau|_x$ of an observer at $x$, relative to the
rescaled ordering coordinate; that reading requires the cone–capacity identification [H-cone] of TempProj (not
derived) and the postulate below.

The local capacity radius is linked, as a declared postulate, to a supplied Lorentzian metric by:

$$R(x)^2 = \frac{g_{\tau\tau}(x)}{g_{\tau\tau}^\infty},$$

where the flat-space reference $g_{\tau\tau}^\infty = -1/A_\tau^\infty$ is postulated (Q11 leaves $A_\tau$ free).
For a supplied static weak-field metric, $R(x) \approx 1 + \Phi_N(x)/c^2$: this restates the standard
gravitational time dilation formula, which the supplied metric carries, in the capacity language.

## Key features

- The homogeneous case ($R(x) \equiv 1$) reduces to TempProj as a corollary.
- The local capacity radius $R(x)$ is identified metrically with the lapse ratio of a supplied Lorentzian
  co-metric; no source constructs that co-metric (Q5b gives rank three under [H-L] and [H-lift], and Q11 gives
  $g \propto \eta$ only after rescaling $\tau$, under the hypotheses of its Corollary 6.1, with $A_\tau$ free). The open
  problem LC-O2-O1 (derive $R(x)$ directly from $\epsilon(x)$ without a supplied metric) **remains open**: the companion paper LCIIo1
  (`Beau2026lco2o1`) shows that the free-fraction law
  $A_\tau = A_\tau^\infty(1-\epsilon)$ does *not* close it — combined with
  $g^{\tau\tau} = -A_\tau$ it yields $g_{\tau\tau}/g_{\tau\tau}^\infty = 1/(1-\epsilon)$,
  agreeing with $R^2 = 1-\epsilon$ only at $\epsilon = 0$.
- The factorisation $R(x) \times \sqrt{f(2-f)}$ cleanly separates local physics
  from the universal normalised Lorentzian structure.

## Status

- Fibrewise map construction: **structural**
- Fibrewise residual $|F^\tau(x,n)| = R(x)/\gamma$: **proved** under the stated hypotheses; its reading as
  gravitational time dilation is **conditional** on [H-cone] and on a supplied weak-field Lorentzian metric (no
  paper of the programme derives either)
- LC-O2-O1 (derivation of $R(x)$ from $\epsilon(x)$ without a supplied metric): **open**.
  The equivalence of the capacity and metric definitions of $R(x)$ (Remark 3.2) is an
  explicitly declared **postulate**, physically coherent and consistent with the
  Schwarzschild weak-field limit, but not derived. LCIIo1 (`Beau2026lco2o1`)
  establishes a no-go for the free-fraction reduction

## Position in the sub-programme

```
LorCap → TempProj → LCII
```

## Dependencies

| Paper | Role |
|-------|------|
| TempProj (`Beau2026tp`) | Flat-space baseline (homogeneous case) |
| LorCap (`Beau2026n`) | Origin of LC-O2 open problem |
| Q5b (`Beau2026q5b`) | Effective operator, co-metric, Carnot geometry |
| Q11 (`Beau2026q11`) | $A_\tau$ free; $g \propto \eta$ after rescaling $\tau$, under the hypotheses of Cor. 6.1 ([H-L], [H-lift], a supplied full-rank extension with [T] and [INV$^+$] of Q8, [ACT$_\tau$] invariance, a negative ordering term) |
| Gravity/H (`Beau2026h`) | Einstein term on a supplied Riemannian metric; supplies no Lorentzian $g_{\tau\tau}(x)$ |
| BI (`Beau2026c`) | Born-Infeld admissibility budget |
| Foundation (`Beau2026m`) | Structural axioms |

## Repository Contents

```
lc-o2/
├── out/              # Compiled PDF
├── tex/
│   ├── lc-o2.tex
│   └── cosmochrony-bibliography.bib
├── compile.sh
├── zenodo.json
└── README.md
```

## Citation

> J. Beau, *Fibrewise Born-Infeld Capacity Lapse and Gravitational Time Dilation*,
> Preprint, 2026.

## Acknowledgements

Portions of the editorial refinement benefited from iterative interactions with
large language models used as analytical assistants.
All claims, interpretations, and final formulations remain the sole
responsibility of the author.
