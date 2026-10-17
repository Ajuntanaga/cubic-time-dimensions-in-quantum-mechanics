# Cubic Time Dimensions in Quantum Mechanics

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23435551.svg)](https://doi.org/10.5281/zenodo.23435551)

This repository tracks the paper lineage and the Chronowave Dynamics compendium module most
directly connected to it, so the two can be versioned together.

## Contents

- `Cubic_Time_Dimensions_in_Quantum_Mechanics_2nd_edition.pdf` — the initial 2nd edition.
- `Cubic_Time_Dimensions_in_Quantum_Mechanics_2nd_edition_combined.pdf` — the revised 2nd edition,
  combined with the companion note *Where Cubic Time Lives* as a single document. Authors: Anthony
  M. Vargas, Lyra R. Novak, Aethus Samir-Iqbal.
- `Module_VIII_Temporal_Hydrogen.html` — Module VIII, "Temporal hydrogen → two-clock periodic
  table," extracted standalone from the full Chronowave Dynamics Temporal Engine compendium. This
  is the module the paper's atom-as-slowed-clock construction, clock-law measurement, and
  118-element ledger are built on. Self-contained: open directly in a browser, no build step.
- `Module_VIII_Manual.md` — a plain-text companion to the HTML above, covering the same material
  as prose for reading without a browser.

## Provenance

Module VIII was extracted from a larger single-file compendium (17 modules in one HTML artifact)
by tracing which interactive elements and JavaScript the module actually depends on, since the
source file's script isn't organized per module. Verified via a headless Node.js harness: the
extracted script parses cleanly, every element ID referenced resolves, and the live-updating
equation panels produce numerically correct results across several elements (hydrogen, uranium,
polonium) that match the published paper's own figures.

The combined paper merges the revised 2nd edition with its companion note via
`scripts/combine_papers.py` (not included here; see the compendium project), renumbering sections,
worked examples, figures, and references rather than dropping any content.

## Citation

See [CITATION.cff](CITATION.cff) (also used by GitHub's "Cite this repository" button).

## License

MIT, see [LICENSE](LICENSE).
