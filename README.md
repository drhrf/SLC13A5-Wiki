# SLC13A5 Evidence Synthesis Wiki

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)

A structured epistemic knowledge graph for SLC13A5 (NaCT, sodium-coupled citrate transporter), built as the proof-of-concept application of a generalizable framework for hypothesis generation in rare disease research.

**Reference paper:** Freitas HR et al. "A structured epistemic knowledge graph for hypothesis generation in rare disease research: proof of concept in SLC13A5 citrate transporter disorder (DEE25)." *Orphanet Journal of Rare Diseases* (under review). Preprint: [bioRxiv DOI — to be added at submission]

---

## What this repository contains

The wiki organizes all available evidence about SLC13A5 into 27 structured nodes across four epistemic tiers, plus five synthesis files that derive cross-domain connections, hypotheses, and a prioritized research agenda from those nodes.

Every substantive claim in every node file carries an explicit epistemic label:

- **Established** — supported by at least two independent studies using different methods; no credible contrary evidence
- **Emerging** — supported by at least one adequately-powered primary study; not yet independently replicated or replicated only in a related system
- **Speculative** — mechanistically motivated and internally coherent, but resting on inference from different systems, developmental stages, or species; no direct measurement in the relevant context
- **Unknown** — the relevant measurement has not been made; the question is open rather than contested

Internal contradictions between sources are not averaged into a single label. They are registered explicitly in `SLC13A5-Wiki/Tier2-Pathways/CONTESTED-CLAIMS.md` with both sources, mechanism-level reasoning, and the evidence needed for resolution.

---

## Repository structure

```
├── FRAMEWORK-SPEC.md           generalizable specification — apply to any gene
├── edge-map.csv                machine-readable adjacency list of all edges
│
└── SLC13A5-Wiki/
    ├── 00-INDEX.md             master node index with directed graph (Mermaid)
    ├── EDGE-MAP.md             confirmed and inferred edges + top connection gaps
    ├── HYPOTHESES.md           12 testable hypotheses across three epistemic tiers
    ├── RESEARCH-AGENDA.md      prioritized studies by time horizon
    ├── MISSING-LINKS.md        unverified citations and open cross-references
    │
    ├── Tier1-Molecular/        what SLC13A5 is and how it works (6 nodes)
    ├── Tier2-Pathways/         how NaCT participates in cellular pathways (11 nodes + contested claims)
    ├── Tier3-Phenotypes/       clinical and organismal consequences of NaCT loss (6 nodes)
    └── Tier4-DiseaseConnections/  adjacent disease hypotheses (4 nodes)
```

---

## Where to start

If you are a **DEE25 / SLC13A5 researcher**, start with `SLC13A5-Wiki/00-INDEX.md` for an overview of the entire evidence graph, then navigate directly to the tier most relevant to your work.

If you want to **apply this framework to a different gene**, start with `FRAMEWORK-SPEC.md`. It contains the complete tier definitions, epistemic label decision rules, node file template, YAML frontmatter schema, edge mapping protocol, and hypothesis classification rubric — everything needed to build a wiki for a different under-characterized rare disease gene without consulting the authors.

If you are reviewing the **reference paper**, the synthesis files (`HYPOTHESES.md`, `EDGE-MAP.md`, `CONTESTED-CLAIMS.md`) correspond to the Results section. The `FRAMEWORK-SPEC.md` corresponds to the Methods section.

---

## The gene: SLC13A5 / NaCT

SLC13A5 encodes NaCT (sodium-coupled citrate transporter), the primary route for plasma citrate uptake into cells. It is expressed most highly in liver and brain. Biallelic loss-of-function variants cause DEE25 (developmental and epileptic encephalopathy 25; OMIM 615905), a severe neonatal encephalopathy characterized by treatment-resistant seizures, intellectual disability, and dental enamel hypoplasia. The gene sits at an unusual intersection: a rare neonatal disease at one end, NaCT inhibitors in late preclinical development for metabolic disease at the other, and an emerging connection to neurodegeneration in the middle. The wiki was built to surface the mechanistic connections between these programs and identify the experiments most urgently needed before any NaCT inhibitor proceeds to human trials.

---

## Tier summary

| Tier | Focus | Nodes |
|------|-------|-------|
| Tier 1 — Molecular | Gene structure, protein, expression, variants, orthologs, interactors | 6 |
| Tier 2 — Pathways | TCA integration, acetyl-CoA production, histone acetylation, hepatic lipid metabolism, NMDA modulation, GABA metabolism, mitochondrial bioenergetics, zinc-citrate interaction, anaplerosis, transcriptional regulation, mTOR signaling | 11 |
| Tier 3 — Phenotypes | Neonatal epilepsy, intellectual disability, movement abnormalities, tooth enamel hypoplasia, hepatic metabolic phenotype, urinary metabolomics signature | 6 |
| Tier 4 — Disease connections | Alzheimer's disease, metabolic syndrome, neurodegeneration broadly, cancer metabolism | 4 |

---

## How to cite

**The framework (this repository):**
> Freitas HR et al. (2026). SLC13A5 Evidence Synthesis Wiki, v1.0. Zenodo. https://doi.org/10.5281/zenodo.XXXXXXX

**The reference paper:**
> Freitas HR et al. (2026). A structured epistemic knowledge graph for hypothesis generation in rare disease research: proof of concept in SLC13A5 citrate transporter disorder (DEE25). *Orphanet Journal of Rare Diseases*. [DOI to be assigned]

If you apply the framework specification to a different gene, please cite the reference paper and note the gene and disease in your acknowledgments.

---

## License

All documentation and knowledge content in this repository is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the material for any purpose, provided you give appropriate credit, link to the license, and indicate if changes were made.

---

## Versioning and updates

This repository is versioned semantically. Each GitHub release is automatically archived to Zenodo with its own DOI. The concept DOI above always resolves to the latest version. See `FRAMEWORK-SPEC.md` for the version release protocol, including the criteria for epistemic label upgrades and what triggers a new release.

| Version | Date | Notes |
|---------|------|-------|
| v1.0 | 2026-05-10 | Initial public release — manuscript submission |
