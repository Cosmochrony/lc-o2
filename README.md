# Gravitational Time Dilation from Position-Dependent Spectral Budget (LC-O2)

This repository contains the source of the paper
*Gravitational Time Dilation from Position-Dependent Spectral Budget:
Non-Uniform Extension of the Temporal Residual Map*
(LC-O2 of the Cosmochrony / spectral admissibility programme).

## Status

**Work in progress** — skeleton only.

## Open problem addressed

LC-O2 is defined in the temporal-projection paper (`Beau2026tp`):

> In non-uniform regimes, position-dependent modifications of the local spectral
> budget encode gravitational time dilation (Remark 2 of `Beau2026n`).
> The flat-space construction of `Beau2026tp` provides the baseline for this extension.

## Intended contribution

Extend the temporal residual map $\mathcal{P}_\tau^{\mathrm{Q5b}}$
from the homogeneous case (uniform Born-Infeld budget) to position-dependent regimes:

$$\Sigma_n^\tau(x) = \mathcal{P}_\tau^{\mathrm{Q5b}}(x)\,\Sigma_n^{\mathrm{tot}}(x)$$

where the local budget varies with the effective position $x$ on
$\mathbb{R}_\tau \times \mathrm{Heis}_3(\mathbb{R})$.
The ratio $\Sigma_n^\tau(x)/\Sigma_n^\tau(y)$ should recover the gravitational
redshift factor between projected histories at $x$ and $y$,
connecting to the IR Einstein response of the gravity paper (`Beau2026h`).

## Dependencies

| Paper | Role |
|-------|------|
| temporal-projection (`Beau2026tp`) | Flat-space baseline construction |
| LorCap (`Beau2026n`) | Origin of LC-O2 open problem |
| Q5b (`Beau2026q5b`) | Effective operator and co-metric |
| Q11 (`Beau2026q11`) | Co-metric completion $g^{\mu\nu} = 2\eta^{\mu\nu}$ |
| Gravity/H (`Beau2026h`) | IR Einstein response — expected connection |
| BI (`Beau2026c`) | Born-Infeld admissibility budget |
| Foundation (`Beau2026m`) | Structural axioms |

## Repository Contents

```
lc-o2/
├── out/              # Compiled PDF
├── tex/              # LaTeX source
│   ├── lc-o2.tex
│   └── cosmochrony-bibliography.bib
├── compile.sh
├── zenodo.json
└── README.md
```
