---
tags: [slc13a5-wiki, tier-2, pathway, mitochondria, OXPHOS, bioenergetics, WGCNA, aging, co-expression]
tier: 2
node_type: pathway
epistemic_status: emerging
last_updated: 2026-05-10
linked_nodes:
  - "[[T1-ExpressionAtlas]]"
  - "[[T2-CitrateTCAIntegration]]"
  - "[[T2-TranscriptionalRegulation]]"
  - "[[T4-AlzheimerDisease]]"
  - "[[T4-NeurodegenerationBroadly]]"
hypothesis_seeds:
  - "The SLC13A5 OXPHOS co-expression module (Ferreira-2026) degrades in AD brain — testable by computing the module eigengene in ROSMAP and SEA-AD data; if it does, SLC13A5 is part of the bioenergetic failure of neurodegeneration"
  - "TFAM-driven mitochondrial biogenesis co-regulates SLC13A5 expression in brain — loss of TFAM activity in aging could be the driver of both OXPHOS decline and SLC13A5 decline in the aging cerebrum"
open_questions:
  - "Does the WGCNA turquoise module from Ferreira-2026 show reduced eigengene in AD brain tissue (ROSMAP DLPFC) relative to age-matched cognitively normal controls — directly testing whether the bioenergetic module SLC13A5 belongs to is disrupted in AD?"
  - "Is TFAM expression positively correlated with SLC13A5 expression in human brain across the lifespan, and does TFAM decline with aging in the same cortical regions where SLC13A5 declines?"
  - "Does NaCT loss in neurons reduce mitochondrial membrane potential or respiratory chain activity — directly, not just through reduced AMPK activation (which is the hepatocyte story)?"
---

# Mitochondrial Bioenergetics and SLC13A5 Co-expression

## Core claim

In human cerebrum, SLC13A5 is embedded in a gene co-expression module whose primary functional signature is oxidative phosphorylation (OXPHOS) and mitochondrial bioenergetics. This module is enriched for genes regulated by TFAM (master mitochondrial transcription regulator) and NFE2/NRF-like motifs (antioxidant response). KEGG pathway enrichment of this module includes Alzheimer's, Parkinson's, and Huntington's disease pathways alongside OXPHOS — reflecting the shared mitochondrial dysfunction that characterizes these diseases. This co-expression is the main bridge from SLC13A5 to adult neurodegeneration. Sources: [[research/Ferreira-2026]], [[mechanisms/mitochondrial-OXPHOS-coexpression]].

## Mechanism

**The co-expression basis (✅ Established as co-expression; ❓ mechanistic causality unknown):**
Ferreira-2026 performed signed WGCNA on Evo-Devo human cerebrum transcriptomes (4 wpc to 63 years, n=22 developmental time points). SLC13A5 was placed in the "turquoise" module — a large module (exact gene count not specified in vault) with:

- Module eigengene tracks developmental rank (ρ = 0.802) and SLC13A5 expression itself (ρ = 0.884)
- Partial correlation between eigengene and SLC13A5, controlling for developmental rank: ρ = 0.672 (p = 6.17 × 10⁻⁴) — SLC13A5 is not just dragged by brain maturation; it is an integrated module member
- GO enrichment: aerobic electron transport chain, respiratory electron transport chain, ATP synthesis coupled electron transport, mitochondrial ATP synthesis — all OXPHOS
- KEGG: oxidative phosphorylation; co-enriched Parkinson's disease, Alzheimer's disease, Huntington's disease, type I diabetes, NAFLD
- TF target enrichment: NFE2/NRF-like (mitochondrial and antioxidant response), TFAM-associated genes (master mitochondrial transcription factor), AP-1 family, ELF1/BACH2

**Why KEGG shows neurodegeneration pathways:**
These KEGG disease annotations are heavily populated with mitochondrial OXPHOS genes — because OXPHOS dysfunction is central to all three diseases. Any module enriched for OXPHOS will appear enriched for these KEGG disease annotations by construction. The wiki must not overstate this as evidence that SLC13A5 causes Alzheimer's or Parkinson's disease.

**What this does show:**
The bioenergetic regulatory neighborhood in which SLC13A5 expression is embedded in human cerebrum is the same neighborhood that is disrupted in adult neurodegeneration. If this co-expression reflects shared transcriptional regulation (TFAM, NRF2-family), then any process that degrades the mitochondrial regulatory program in aging (well established in AD, PD, HD) would be expected to reduce SLC13A5 expression alongside OXPHOS genes as a passenger.

**Hepatocyte AMPK-mitochondrial biogenesis cascade (✅ Established):**
In hepatocytes (Birkenfeld-2011), NaCT loss → reduced ATP/ADP ratio → AMPK → PGC-1α → mitochondrial biogenesis. This is a direct perturbational demonstration that NaCT activity affects mitochondrial biogenesis in hepatocytes. Whether a comparable cascade operates in neurons — where the citrate flux through NaCT is lower and the metabolic consequences of NaCT loss differ — is not established in the vault.

**Perturbational corroboration (Fan-2021):**
Nervous-system-specific mINDY deletion in adult mice improves cognition and motor performance, phenocopying dietary restriction. Dietary restriction activates AMPK and mitochondrial biogenesis — suggesting the brain NaCT-AMPK-mitochondria cascade observed in liver also operates in brain, though not directly measured.

## Evidence basis

- Source 1: [[research/Ferreira-2026]] — WGCNA analysis; module eigengene tracking; GO/KEGG/TF enrichment; network nucleus with SLC13A5 adjacent to GABA and nAChR associated genes.
- Source 2: [[mechanisms/mitochondrial-OXPHOS-coexpression]] — detailed mechanistic page for this finding; contains critical caution against over-interpreting KEGG disease enrichment.
- Source 3: [[research/Birkenfeld-2011]] — hepatocyte AMPK-PGC1α-mitochondrial biogenesis cascade downstream of NaCT loss; perturbational evidence in liver.
- Source 4: [[research/Fan-2021]] — brain-specific mINDY deletion cognitive benefit; consistent with mitochondrial biogenesis activation hypothesis but not directly measured.

## Connections to other nodes

- [[T1-ExpressionAtlas]] — the WGCNA module that contains SLC13A5 also defines the developmental trajectory of co-expressed genes; the module's rise and fall parallels SLC13A5 cerebrum expression.
- [[T2-CitrateTCAIntegration]] — NaCT-imported citrate feeds TCA-cycle flux that supports mitochondrial function; there is a bidirectional relationship between NaCT activity and mitochondrial bioenergetic state.
- [[T2-TranscriptionalRegulation]] — TFAM and NRF-like factors inferred as brain-side regulators of SLC13A5 from the module TF enrichment; this connects transcriptional regulation to the bioenergetic context.
- [[T4-AlzheimerDisease]] — the central connection: OXPHOS module containing SLC13A5 may degrade in AD, placing SLC13A5 as a passenger or driver of bioenergetic failure in neurodegeneration.
- [[T4-NeurodegenerationBroadly]] — broader than AD; the KEGG enrichment includes PD and HD, suggesting the bioenergetic module is a shared vulnerability point across neurodegenerative diseases.

## Open questions

1. Does the WGCNA turquoise module (SLC13A5 module from Ferreira-2026) show reduced eigengene in ROSMAP DLPFC AD vs. control samples — the most direct test of whether this bioenergetic module is disrupted in AD?
2. Is TFAM expression positively correlated with SLC13A5 in human cerebrum across the lifespan — specifically, does TFAM decline in late aging in the same cortical regions where SLC13A5 declines, consistent with shared transcriptional regulation?
3. Does NaCT loss in neurons directly reduce mitochondrial membrane potential (ΔΨm) or Complex I activity — rather than indirectly through AMPK, which is the hepatocyte mechanism? This could be measured in DEE25 iPSC neurons by JC-1 staining or Seahorse respirometry.
4. What are the specific hub genes of the Ferreira-2026 turquoise module — and are they the same genes that appear as top differentially expressed in AD, PD, or HD transcriptomic studies? This would distinguish a true module-level overlap from incidental KEGG annotation overlap.
