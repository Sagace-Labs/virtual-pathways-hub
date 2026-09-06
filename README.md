# Virtual Pathways

Independently published molecular predictors for liver safety and drug metabolism.
Each pathway package turns a SMILES string into assay, substrate-label,
site-of-metabolism or candidate-metabolite predictions.

| Repository | Package | Current release | Predicts |
|---|---|---|---|
| [vp-core](https://github.com/Sagace-Labs/vp-core) | `vp-core` 1.7.0 | — | Shared splits, featurisers, metrics, evaluation protocols and the version manifest schema |
| [vp-bsep](https://github.com/Sagace-Labs/vp-bsep) | `vp-bsep` 2.0.0 | v2 | BSEP / ABCB11 inhibition, the initiating event for cholestatic liver injury |
| [vp-oxphos](https://github.com/Sagace-Labs/vp-oxphos) | `vp-oxphos` 2.1.0 | v3 | Mitochondrial membrane-potential disruption, with its viability counter-screen |
| [vp-nrf2](https://github.com/Sagace-Labs/vp-nrf2) | `vp-nrf2` 1.2.0 | v3 | NRF2 / KEAP1 antioxidant-response activation, with its viability counter-screen |
| [vp-ahr](https://github.com/Sagace-Labs/vp-ahr) | `vp-ahr` 1.0.0 | v1 | Aryl hydrocarbon receptor activation, with its viability counter-screen |
| [vp-gr](https://github.com/Sagace-Labs/vp-gr) | `vp-gr` 1.0.0 | v1 | Glucocorticoid receptor agonism and antagonism, with its viability counter-screen |
| [vp-hsr](https://github.com/Sagace-Labs/vp-hsr) | `vp-hsr` 1.0.0 | v1 | Heat shock response activation, with its viability counter-screen |
| [vp-p53](https://github.com/Sagace-Labs/vp-p53) | `vp-p53` 1.0.0 | v1 | p53 genotoxic stress response activation, with its viability counter-screen |
| [vp-pxr](https://github.com/Sagace-Labs/vp-pxr) | `vp-pxr` 1.0.0 | v1 | Pregnane X receptor activation, with its viability counter-screen |
| [vp-cyp-inhibition](https://github.com/Sagace-Labs/vp-cyp-inhibition) | `vp-cyp-inhibition` 1.0.0 | v1 | Predicts whether a molecule reduces CYP1A2, CYP2C9, CYP2D6 or CYP3A4 activity by at least half in a 50 µM assay |
| [vp-cyp-substrate](https://github.com/Sagace-Labs/vp-cyp-substrate) | `vp-cyp-substrate` 1.0.0 | v1 | Predicts whether a molecule is a substrate of CYP1A2, CYP2C9, CYP2D6 or CYP3A4 |
| [vp-som](https://github.com/Sagace-Labs/vp-som) | `vp-som` 1.0.0 | v1 | Ranks pooled CYP oxidative sites, one score per atom |
| [vp-metabolite](https://github.com/Sagace-Labs/vp-metabolite) | `vp-metabolite` 1.0.0 | v1 | Ranks candidate xenobiotic metabolite structures from a parent SMILES |

## Datasets

Dataset repositories publish processed tables, source attribution and rebuild
instructions.

| Repository | Package | Current release | Contents |
|---|---|---|---|
| [data-xenobiotic-metabolism](https://github.com/Sagace-Labs/data-xenobiotic-metabolism) | `data-xenobiotic-metabolism` 0.1.0 | v1 | Directed xenobiotic parent–metabolite pairs from five attributed sources |

## Clone

Install Git LFS for the metabolite weights before cloning.

    git lfs install
    git clone --recurse-submodules https://github.com/Sagace-Labs/virtual-pathways-hub.git

Packages install from their individual repositories and depend on `vp-core`.

## Data and licences

A version records the origin of the data, the date, the licence, and the
hash of the standardised table. Re-fetching re-hashes.

Code is Apache-2.0 unless a package states otherwise. `vp-metabolite` is
GPL-3.0 because its bundled transformation rules are GPL-3.0. A package that
bundles a dataset carries a separate `LICENSE-DATA` stating the source terms.
