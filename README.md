# APEPM-Model-pre-QM-geometric-bond-feasibility-screening-and-bond-visualizer
This code implements the APEPM model found on chemrxiv, and is intended to ideally be used either as a pre-QM screening method to see if bonds are geometrically possible (not energetically)(if overlap radius = 0, then there can be no bond), or see if a bond is possible at all based on distance between electron radii of 2 atoms. APEPM model paper available here: https://doi.org/10.26434/chemrxiv-2026-9swcr


# Please Note:
This model and paper relies on AREECM notation, the code already comes with the digital AREECM dictionary, but for the "+1" rule seen here that applies to AREECM notation, for a better understanding of AREECM, the AREECM paper can be found here on chemrxiv: https://doi.org/10.26434/chemrxiv-2025-jq84z-v3


# Industrial Uses/Applications

APEPM offers a wavefunction-free, analytic evaluation of whether two atomic electron volumes can share non-zero overlap as defined in the ChemRxiv model paper https://doi.org/10.26434/chemrxiv-2026-9swcr
In automated discovery pipelines, this enables early rejection or annotation of structures that are geometrically incapable of bonding before QM, DFT, or ML potentials are executed.

# Capabilities

Deterministic identification of infeasible or highly strained bonds based solely on geometry

Millisecond-scale assessment for molecules, clusters, and periodic fragments

Closed-form, non-iterative calculations with no SCF or convergence tuning

Use as an interpretable constraint or weighting layer inside custom energy models

Real-time generation of orbital-overlap visualizations (e.g., Au···Au metallophilic contacts, U=O actinyl bonds, metal–oxo motifs) without requiring QM density cube files

# Workflow Example

Candidate Geometry → APEPM Screening → QM / DFT / ML on admissible bonds

# Summary

APEPM separates geometric admissibility from energetic favorability, providing structural context and reducing wasted downstream computation in high-throughput industrial workflows.

# Licensing

The repository and associated papers are released under CC BY-NC 4.0. Commercial deployment or integration requires a dedicated license agreement from the owner.
