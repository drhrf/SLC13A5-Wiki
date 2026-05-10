---
tags: [slc13a5-wiki, tier-4, disease, Alzheimer, dementia, cholinergic, OXPHOS, biomarker, aging, neurodegeneration]
tier: 4
node_type: disease-connection
epistemic_status: speculative-to-emerging
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-AcetylCoAProduction]]"
  - "[[T2-MitochondrialBioenergetics]]"
  - "[[T2-HistoneAcetylation]]"
  - "[[T3-UrinaryMetabolomicsSignature]]"
  - "[[T1-ExpressionAtlas]]"
hypothesis_seeds:
  - "Declining cerebral SLC13A5 expression in aging crosses a threshold in the 7th-8th decade that constrains ACLY-derived acetyl-CoA supply to cholinergic neurons, contributing to the cholinergic deficit that defines Alzheimer's disease"
  - "The Ferreira-2026 turquoise OXPHOS-SLC13A5 co-expression module eigengene will be significantly reduced in ROSMAP AD DLPFC samples compared to age-matched cognitively normal controls — directly linking the SLC13A5 co-expression neighborhood to AD molecular pathology"
  - "Mendelian randomization using SLC13A5 DMS functional scores as instruments for plasma citrate will yield a causal estimate of elevated plasma citrate on AD risk, implicating common SLC13A5 variant effects in pre-dementia risk stratification"
open_questions:
  - "Is SLC13A5 expressed in ChAT-positive cholinergic neuron clusters in the Allen Brain Cell Atlas — the most direct test of the cholinergic vulnerability hypothesis?"
  - "Does the Ferreira-2026 WGCNA turquoise module eigengene decline in AD brain tissue in ROSMAP bulk RNA-seq, and does SLC13A5 track this decline or deviate from it?"
  - "Is there a non-linear (U-shaped) relationship between SLC13A5 DMS functional score and cognitive performance in UK Biobank — testing whether NaCT activity has an optimal range rather than a monotone relationship with cognition?"
---

# SLC13A5 and Alzheimer's Disease

## Core claim

The link between SLC13A5 and Alzheimer's disease (AD) is a mechanistically motivated research hypothesis, not an established causal connection. It is supported by four converging evidence layers: (1) co-expression of SLC13A5 with OXPHOS genes in a brain module enriched for AD pathways (Ferreira-2026); (2) cognitive benefit of brain NaCT reduction in adult mice that mimics dietary restriction (Fan-2021); (3) rising CSF citrate with normal aging and plasma citrate predicting pre-dementia cognitive decline (Lin-2021, Tremblay-Franco-2024); (4) ACLY as the primary source of acetyl-CoA for ACh synthesis in cholinergic neurons (Gul-Hinc-2026) — establishing the biochemical chain from citrate supply to cholinergic function. None of these layers directly demonstrates NaCT dysfunction in human AD brain. Sources: [[research/Ferreira-2026]], [[research/Fan-2021]], [[research/Lin-2021]], [[research/Tremblay-Franco-2024]], [[research/Gul-Hinc-2026]], [[research/Pourshafie-2026]], [[research/Hofling-2026]], [[research/Wang-2025]].

## Mechanism

**Layer 1 — Co-expression bridge (🔶 Emerging — Ferreira-2026):**
WGCNA on the Evo-Devo human transcriptome dataset places SLC13A5 in the turquoise module — the largest and most stable module in the adult brain network. The turquoise module is characterized by:
- Functional enrichment: oxidative phosphorylation, mitochondrial electron transport chain, citrate cycle
- KEGG pathway enrichment: Alzheimer's disease, Parkinson's disease, Huntington's disease
- TF enrichment: TFAM-associated genes and NFE2/NRF-like motifs (mitochondrial biogenesis regulators)
- Temporal trajectory: module eigengene tracks brain maturation; cerebral SLC13A5 peaks in the first postnatal year then declines

This co-expression bridge is correlational: it does not demonstrate that SLC13A5 is specifically dysregulated in AD brain. It establishes that SLC13A5 is embedded in the mitochondrial bioenergetic gene neighborhood whose degradation is a known feature of AD pathology.

**Layer 2 — Perturbational evidence (🔶 Emerging — Fan-2021):**
Nervous-system-specific deletion of mIndy (mouse Slc13a5) in adult mice improves spatial memory (Morris water maze), recognition memory (novel object recognition), and motor coordination (accelerating rotarod) relative to littermate controls. The cognitive benefit persists for at least 6 months and is brain-specific (not secondary to hepatic metabolic changes). The magnitude of improvement parallels dietary restriction — the most robust cognitive-preservation intervention in rodents.

The Fan-2021 finding is counterintuitive: *reducing* brain NaCT improves cognition. The reconciling hypothesis is a U-shaped NaCT-cognition relationship: reduction from a high young-adult baseline is beneficial (dietary-restriction mimicry via AMPK-mTOR suppression, autophagy induction); reduction from an already-low aging baseline would be harmful. This hypothesis is untested. The species-capacity difference (mouse Slc13a5 is low-capacity; human SLC13A5 is high-capacity) means that the "high baseline" in young adult mice is far lower than the equivalent baseline in young adult humans.

**Layer 3 — Citrate as biomarker (🔶 Emerging — Lin-2021, Tremblay-Franco-2024, Hofling-2026):**

*Lin-2021*: CSF citrate rises continuously with age in 75 cognitively unimpaired adults (ages 20–92). This rise is part of a five-metabolite aging signature interpreted as reflecting declining mitochondrial function — consistent with reduced citrate clearance from the extracellular space as NaCT activity declines with age.

*Tremblay-Franco-2024*: Plasma citrate (as part of a TCA cycle metabolite panel) predicts future cognitive decline in amyloid-positive pre-dementia subjects. This is the most direct human evidence linking citrate to AD-trajectory prediction. The mechanism is not established — the elevated plasma citrate could reflect reduced cellular citrate uptake (NaCT hypofunction) or increased citrate production or reduced mitochondrial processing.

*Hofling-2026*: CSF citric acid is specifically reduced in idiopathic normal pressure hydrocephalus (iNPH) relative to AD/MCI/FTD (AUC 0.97 in a discriminative panel). This implies AD/MCI/FTD do not have reduced CSF citrate — the age-related rise in normals (Lin-2021) may persist into early AD dementia.

**Layer 4 — ACLY-cholinergic biochemical chain (✅ Established for the ACLY step — Gul-Hinc-2026):**
Gul-Hinc-2026 establishes that ACLY is the primary source of acetyl-CoA for acetylcholine synthesis in cholinergic neurons. ACLY localizes at presynaptic terminals, co-localizes with ChAT (choline acetyltransferase), and its expression correlates with ChAT activity across brain regions. Cholinergic deficit is the hallmark of Alzheimer's disease and the mechanism targeted by acetylcholinesterase inhibitors (standard of care). If SLC13A5 activity declines in cholinergic neurons, less citrate reaches ACLY, constraining acetyl-CoA supply to ACh synthesis. The chain NaCT → citrate → ACLY → acetyl-CoA → ACh is biochemically coherent. Direct evidence that SLC13A5 decline in human cholinergic neurons precedes or accompanies AD pathology is absent from the vault.

Pourshafie-2026 adds a parallel route: ACSS2 → acetate → nuclear acetyl-CoA → histone acetylation at synaptic gene loci protects neurons from tau-driven cognitive decline. Reduced nuclear acetyl-CoA (from either ACLY or ACSS2 hypofunction) impairs neuroprotective gene expression. Both pathways converge on the same nuclear pool.

**Population-scale functional data (✅ Established for citrate-NaCT correlation — Wang-2025):**
Deep mutational scanning (DMS) of SLC13A5 variants produces functional scores for 9,707 of 10,773 possible substitutions. DMS score negatively correlates with blood citrate in UK Biobank (r = −0.63 for alleles with minor allele count >25). This validates blood citrate as a proxy for NaCT activity at the population level and enables Mendelian randomization studies testing whether citrate causally affects AD risk.

## Evidence basis

- Source 1: [[research/Ferreira-2026]] — WGCNA turquoise module; AD pathway enrichment; SLC13A5 temporal trajectory; TF enrichment.
- Source 2: [[research/Fan-2021]] — brain-specific mIndy deletion; cognitive benefit; dietary restriction mimicry.
- Source 3: [[research/Lin-2021]] — CSF citrate rising with age in 75 cognitively unimpaired adults.
- Source 4: [[research/Tremblay-Franco-2024]] — plasma citrate in TCA panel predicts cognitive decline in amyloid-positive pre-dementia subjects.
- Source 5: [[research/Hofling-2026]] — CSF citric acid discriminates iNPH from AD/MCI/FTD; AD does not have reduced CSF citrate.
- Source 6: [[research/Gul-Hinc-2026]] — ACLY as primary ACh acetyl-CoA source; cholinergic region-level correlation; presynaptic terminal localization.
- Source 7: [[research/Pourshafie-2026]] — ACSS2 nuclear acetyl-CoA → histone acetylation → neuroprotection against tau.
- Source 8: [[research/Wang-2025]] — DMS functional scores; blood citrate-NaCT correlation in UK Biobank.

## Connections to other nodes

- [[T2-AcetylCoAProduction]] — the ACLY→ACh and ACLY→histone acetylation pathway is the central mechanistic link between NaCT and cholinergic vulnerability.
- [[T2-MitochondrialBioenergetics]] — the OXPHOS co-expression module that houses SLC13A5 is the co-expression basis of the AD connection.
- [[T2-HistoneAcetylation]] — nuclear acetyl-CoA for synaptic gene regulation is the epigenetic arm of the AD connection.
- [[T3-UrinaryMetabolomicsSignature]] — citrate as a biomarker spans both DEE25 diagnosis and AD pre-dementia prediction.
- [[T1-ExpressionAtlas]] — the declining cerebral SLC13A5 trajectory in postnatal life is the expression basis of the aging-decline hypothesis.

## Open questions

1. Is SLC13A5 expressed in ChAT-positive neuronal clusters in the Allen Brain Cell Atlas — the single most informative query for the cholinergic vulnerability hypothesis?
2. Does the Ferreira-2026 turquoise module eigengene decline in ROSMAP AD DLPFC samples, and does SLC13A5 decline in proportion or independently?
3. Is SEA-AD single-nucleus RNA-seq showing SLC13A5 downregulation in excitatory or cholinergic neurons in AD cases relative to age-matched controls?
4. Do Wang-2025 DMS functional scores for SLC13A5 variants predict cognitive performance in UK Biobank, and is this relationship non-linear?
5. Does Mendelian randomization using DMS-weighted SLC13A5 variants as instruments for plasma citrate yield a causal estimate of citrate's effect on AD risk?
6. Is the Fan-2021 cognitive benefit replicated in aged mice (not young adult), and is the direction reversed (worsening) when mIndy is deleted from an already age-declined expression level?
