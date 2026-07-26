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

**Gravitational time dilation** emerges as:

$$\frac{d\tau}{dn}\bigg|_x = \frac{R(x)}{\gamma}$$

The local capacity radius is linked to the metric by:

$$R(x)^2 = -2\,g_{\tau\tau}(x)$$

In the weak-field regime, $R(x) \approx 1 + \Phi_N(x)/c^2$, recovering the standard
gravitational time dilation formula.

## Key features

- The homogeneous case ($R(x) \equiv 1$) reduces to TempProj as a corollary.
- The local capacity radius $R(x)$ is identified metrically from Q5b/Q11. The open
  problem LC-O2-O1 (derive $R(x)$ directly from $\epsilon(x)$ without importing the
  Einstein equations) **remains open**: the companion paper LCIIo1
  (`Beau2026lco2o1`) shows that the free-fraction law
  $A_\tau = A_\tau^\infty(1-\epsilon)$ does *not* close it — combined with
  $g^{\tau\tau} = -A_\tau$ it yields $g_{\tau\tau}/g_{\tau\tau}^\infty = 1/(1-\epsilon)$,
  agreeing with $R^2 = 1-\epsilon$ only at $\epsilon = 0$.
- The factorisation $R(x) \times \sqrt{f(2-f)}$ cleanly separates local physics
  from the universal normalised Lorentzian structure.

## Status

- Fibrewise map construction: **structural**
- Gravitational time dilation formula: **structural** (imports $g_{\tau\tau}$ from Gravity paper)
- LC-O2-O1 (derivation of $R(x)$ from $\epsilon(x)$ without Einstein equation): **open**.
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
| Q11 (`Beau2026q11`) | Co-metric completion $g^{\mu\nu} = 2\eta^{\mu\nu}$ |
| Gravity/H (`Beau2026h`) | IR Einstein response — provides $g_{\tau\tau}(x)$ |
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
