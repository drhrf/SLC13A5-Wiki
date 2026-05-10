---
tags: [slc13a5-wiki, tier-1, molecular, expression, brain, liver, developmental, lifespan]
tier: 1
node_type: molecular
epistemic_status: established
last_updated: 2026-05-10
linked_nodes:
  - "[[T1-SLC13A5-GeneStructure]]"
  - "[[T2-TranscriptionalRegulation]]"
  - "[[T2-MitochondrialBioenergetics]]"
  - "[[T3-NeonatalEpilepsy]]"
  - "[[T4-AlzheimerDisease]]"
hypothesis_seeds:
  - "The cerebellar SLC13A5 rise across the lifespan may reflect NRF2/TFAM-driven mitochondrial stress response, linking it to ataxia and MSA-C biology"
  - "The cortical expression peak in the first postnatal year defines a critical window during which NaCT-mediated citrate import shapes circuit formation"
open_questions:
  - "Which specific cortical cell types (excitatory vs. inhibitory neurons, layer identity) express SLC13A5 at peak developmental levels — and does the cell-type composition of the expressing population change with age?"
  - "Does SLC13A5 expression in human basal forebrain cholinergic neurons (nucleus basalis, medial septum) decline with age in a pattern relevant to AD?"
  - "Is the cerebellar rising trajectory driven by granule cells, Purkinje cells, or Bergmann glia — and does it reflect increased citrate demand or compensatory upregulation?"
---

# Expression Atlas

## Core claim

SLC13A5 shows the highest expression in liver among all surveyed tissues, with a secondary peak in brain during the first postnatal year that then declines. Cerebellar expression shows the opposite trajectory, rising continuously across the lifespan. Brain cell-type specificity is established at the mRNA level — SLC13A5 is expressed in neurons and likely in specific non-neuronal populations including osteoblasts and ameloblasts. The developmental trajectory of cerebrum expression directly parallels the symptomatic window of DEE25. Sources: [[research/Ferreira-2026]], [[genes/SLC13A5]], [[research/Dirckx-2022]].

## Mechanism

The tissue-specific and developmental expression of SLC13A5 is governed by distinct regulatory programs in different tissues (see [[T2-TranscriptionalRegulation]]). The expression data comes from multiple sources with different coverage and sensitivity:

**Evo-Devo human transcriptomes (Ferreira-2026):** The primary anchor for developmental trajectories.

| Tissue | Expression trajectory |
|--------|----------------------|
| Cerebrum | Rises from ~0.5 RPKM at 19 wpc to peak ~4 RPKM in first postnatal year; declines into adulthood; plateaus >1 RPKM in later decades |
| Cerebellum | Low (<1 RPKM) early; slow continuous rise across lifespan — opposite of cerebrum |
| Liver | Highest of all tissues (~50 RPKM fetal, ~20 RPKM at birth, rises to ~60 RPKM adult) |
| Kidney, ovary, testis | Low throughout life |

**Bone and tooth expression (Dirckx-2022):** SLC13A5 is highly expressed in osteoblasts (comparable to testis), with expression rising during osteoblast differentiation and peaking in mineralizing osteoblasts and osteocytes. Expressed in ameloblasts (enamel-forming) and odontoblasts (dentin-forming). This non-neuronal, non-hepatic expression explains the dental phenotype of DEE25.

**Brain cell-type specificity:** The published single-cell RNA-seq data (Allen Brain Cell Atlas, relevant papers referenced in the [[queries/hypotheses-SLC13A5-dementia-Alzheimer]] and [[queries/hypotheses-SLC13A5-developmental-disorders]] files) suggests SLC13A5 expression in neuronal populations, with the precise cell-type enrichment at the postnatal peak unresolved. The co-expression module analysis by Ferreira-2026 places SLC13A5 adjacent to a GABA-A receptor subunit gene and an nAChR-associated gene in the network nucleus, consistent with expression in GABAergic and/or cholinergic neurons.

**Developmental significance:** The cerebrum SLC13A5 peak in the first postnatal year coincides precisely with the symptomatic window of DEE25 (seizures onset in the first days of life; maximum burden in years 0–3). The decline that follows parallels the observed reduction in seizure burden with age ([[research/Matricardi-2020]]; [[conditions/SLC13A5-deficiency]]), though this is a correlation, not a demonstrated mechanism.

**The cerebellar anomaly:** Lifelong rising cerebellar SLC13A5 expression is a novel observation with no established phenotypic correlate in DEE25 patients. Cerebellar phenotype is not a recognized centerpiece of the disorder. Whether this rising expression represents increased cerebellar citrate demand with aging, a mitochondrial stress-response program engaged more robustly in cerebellum than cerebrum, or an artifact of cell-type composition change, is unresolved.

## Evidence basis

- Source 1: [[research/Ferreira-2026]] — Evo-Devo WGCNA; primary source for tissue trajectories including the cerebellar rise and cerebrum peak-then-decline.
- Source 2: [[genes/SLC13A5]] — integrated expression summary; confirms liver as highest-expressing tissue and notes developmental brain trajectory.
- Source 3: [[research/Dirckx-2022]] — bone and dental expression; osteoblast differentiation trajectory; ameloblast/odontoblast expression.
- Source 4: [[research/Li-Wang-2021]] — reviewed adult tissue expression data confirming liver predominance and low peripheral tissue expression.
- Source 5: [[research/Kopel-2021]] — states brain (neurons) and liver as the two tissues with major functional consequences of NaCT activity.

## Connections to other nodes

- [[T1-SLC13A5-GeneStructure]] — regulatory elements in the gene drive the tissue-specific expression patterns.
- [[T2-TranscriptionalRegulation]] — PXR/AhR drive liver expression; TFAM/NRF-like factors inferred for brain.
- [[T2-MitochondrialBioenergetics]] — SLC13A5 co-expresses with OXPHOS genes in the WGCNA turquoise module, suggesting shared regulatory drivers in cerebrum.
- [[T3-NeonatalEpilepsy]] — cerebrum expression peak during the first postnatal year explains the timing of seizure onset and relative abatement with age.
- [[T4-AlzheimerDisease]] — the cerebrum expression declining with age is the expression-level foundation of the aging-decline hypothesis (H2 in [[queries/hypotheses-SLC13A5-dementia-Alzheimer]]).

## Open questions

1. Which specific cortical layers and neuron types show SLC13A5 expression at the postnatal peak — layer 2/3 excitatory neurons, GABAergic interneurons (PV, SST, VIP subtypes), or a different population? This is directly queryable in the Allen Brain Cell Atlas.
2. Does SLC13A5 expression decline in basal forebrain cholinergic neurons (nucleus basalis of Meynert, medial septal nucleus) with age in a pattern that would predict cholinergic vulnerability — the central prediction of the H1 cholinergic hypothesis in [[queries/hypotheses-SLC13A5-dementia-Alzheimer]]?
3. Is cerebellar SLC13A5 expression enriched in Purkinje cells relative to granule cells — and if so, does Purkinje cell SLC13A5 expression change in spinocerebellar ataxia models?
4. Does the fetal liver SLC13A5 expression drop at birth because liver NaCT activity is replaced by another mechanism, or because fetal hepatic citrate metabolism is genuinely higher than in the neonatal period?
