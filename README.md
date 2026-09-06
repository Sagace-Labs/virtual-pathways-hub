# Virtual Pathways

Pathway-specific molecular predictors for drug-induced liver injury.
Virtual pathways are independently published Python packages that turn a SMILES string
into a prediction about one molecular initiating event.

| Repository | Package | Current release | Predicts |
|---|---|---|---|
| [vp-core](https://github.com/Sagace-Labs/vp-core) | `vp-core` 1.4.0 | — | Shared splits, featurisers, metrics, evaluation protocols and the version manifest schema |
| [vp-bsep](https://github.com/Sagace-Labs/vp-bsep) | `vp-bsep` 2.0.0 | v2 | BSEP / ABCB11 inhibition, the initiating event for cholestatic liver injury |
| [vp-oxphos](https://github.com/Sagace-Labs/vp-oxphos) | `vp-oxphos` 2.1.0 | v3 | Mitochondrial membrane-potential disruption, with its viability counter-screen |
| [vp-nrf2](https://github.com/Sagace-Labs/vp-nrf2) | `vp-nrf2` 1.1.0 | v2 | NRF2 / KEAP1 antioxidant-response activation, with its viability counter-screen |
| [vp-ahr](https://github.com/Sagace-Labs/vp-ahr) | `vp-ahr` 1.0.0 | v1 | Aryl hydrocarbon receptor activation, with its viability counter-screen |
| [vp-gr](https://github.com/Sagace-Labs/vp-gr) | `vp-gr` 1.0.0 | v1 | Glucocorticoid receptor agonism and antagonism, with its viability counter-screen |
| [vp-hsr](https://github.com/Sagace-Labs/vp-hsr) | `vp-hsr` 1.0.0 | v1 | Heat shock response activation, with its viability counter-screen |
| [vp-p53](https://github.com/Sagace-Labs/vp-p53) | `vp-p53` 1.0.0 | v1 | p53 genotoxic stress response activation, with its viability counter-screen |
| [vp-pxr](https://github.com/Sagace-Labs/vp-pxr) | `vp-pxr` 1.0.0 | v1 | Pregnane X receptor activation, with its viability counter-screen |

## Clone

    git clone --recurse-submodules https://github.com/Sagace-Labs/virtual-pathways-hub.git

Packages install on their own from PyPI and depend on `vp-core`.

## Data and licences

A version records the origin of the data, the date, the licence, and the
hash of the standardised table. Re-fetching re-hashes.

Code is Apache-2.0 throughout. A package that bundles a dataset carries a
separate `LICENSE-DATA` stating the source's own terms.
