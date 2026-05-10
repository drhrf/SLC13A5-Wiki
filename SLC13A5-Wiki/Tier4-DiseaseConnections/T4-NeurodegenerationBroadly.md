---
tags: [slc13a5-wiki, tier-4, disease, neurodegeneration, aging, longevity, INDY, mTOR, autophagy, Parkinson, Huntington]
tier: 4
node_type: disease-connection
epistemic_status: speculative
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-MitochondrialBioenergetics]]"
  - "[[T2-mTORSignaling]]"
  - "[[T1-INDYOrthologs]]"
  - "[[T4-AlzheimerDisease]]"
  - "[[T4-MetabolicSyndrome]]"
hypothesis_seeds:
  - "SLC13A5 is a node in the evolutionarily conserved citrate-AMPK-mTOR-autophagy axis that determines cellular aging rate — reduction of NaCT activity is one of several mechanisms by which caloric restriction extends lifespan, and this mechanism is active in mammalian brain as well as invertebrate soma"
  - "The Ferreira-2026 turquoise module KEGG enrichment for Parkinson's and Huntington's disease pathways is not coincidental — it reflects shared OXPHOS/mitochondrial failure pathology, and SLC13A5 expression decline is a feature of the mitochondrial failure common to synucleinopathies and polyglutamine diseases as well as AD"
open_questions:
  - "Does Slc13a5 KO in mice produce any detectable resistance to MPTP-induced dopaminergic neuron loss — a direct test of whether NaCT reduction protects against PD-relevant oxidative stress in substantia nigra neurons?"
  - "In the SEA-AD or other transcriptomic datasets for Parkinson's or Huntington's disease, does SLC13A5 expression track OXPHOS module decline analogously to what is predicted for AD — testing whether the Ferreira-2026 KEGG enrichment reflects actual gene expression changes in these diseases?"
  - "Is SLC13A5 expressed in dopaminergic neurons of the substantia nigra — the selectively vulnerable population in Parkinson's disease — in the Allen Brain Cell Atlas?"
---

# SLC13A5 and Neurodegeneration Broadly

## Core claim

The SLC13A5-neurodegeneration connection extends beyond Alzheimer's disease to encompass the broader theme of mitochondrial bioenergetic failure in neurodegeneration, evolutionary conservation of the INDY longevity pathway, and the mTOR-autophagy axis as a mechanism of NaCT-mediated neuroprotection. The Ferreira-2026 WGCNA turquoise module has KEGG enrichment for Alzheimer's, Parkinson's, and Huntington's disease — not just AD. However, direct evidence for SLC13A5 dysregulation in PD, HD, or other neurodegenerative diseases is absent from the vault. The connection is mechanistically motivated and the OXPHOS co-expression data is a credible starting point, but this node is the most speculative in the wiki. Sources: [[research/Ferreira-2026]], [[research/Fan-2021]], [[research/Kopel-2021]], [[research/Birkenfeld-2011]]; broader neurodegeneration: no vault source directly demonstrates SLC13A5 involvement. Claims are cross-domain inferences.

## Mechanism

**INDY longevity pathway — evolutionary conservation (✅ Established for invertebrates; 🔶 Emerging for mammals):**
The INDY gene in Drosophila (I'm Not Dead Yet) was the founding member of the NaCT family as a longevity gene. Heterozygous INDY loss-of-function extends Drosophila median lifespan 30–50%. C. elegans indy-1 similarly extends lifespan. Mouse mIndy KO on chow extends healthy metabolic lifespan by mimicking caloric restriction. The proposed mechanism: reduced INDY/mINDY activity → reduced citrate import → reduced TCA cycle anaplerosis → reduced ATP/ADP ratio → AMPK activation → reduced insulin/IGF-1 signaling → extended lifespan (paralleling the DR → reduced IIS pathway in model organisms).

In this framework, SLC13A5 is a metabolic node in the conserved aging-rate pathway, not merely a nutrient transporter. Interventions that reduce NaCT activity (genetic loss-of-function, pharmacological inhibition, or natural aging-related expression decline) mimic dietary restriction to varying degrees — with cognitive benefits in adult mice (Fan-2021) representing one manifestation.

**OXPHOS co-expression and multi-disease relevance (🔶 Emerging — Ferreira-2026):**
The turquoise module containing SLC13A5 in Ferreira-2026 has KEGG enrichment for AD, PD, and HD. This is not coincidental: all three diseases share OXPHOS/mitochondrial failure as a core pathological feature. SLC13A5 in this module may reflect a common bioenergetic vulnerability rather than disease-specific biology. Whether SLC13A5 is specifically dysregulated in PD or HD brain tissue — beyond what the OXPHOS module co-expression would predict — is unknown.

**AMPK-mTOR-autophagy axis (💡 Speculative):**
As described in [[T2-mTORSignaling]]: NaCT loss → reduced cytoplasmic citrate → reduced ATP/ADP ratio → AMPK activation → mTORC1 suppression → autophagy induction. Autophagy is essential for clearance of alpha-synuclein (PD), huntingtin aggregates (HD), and tau (AD). A mechanism where reduced NaCT activity induces autophagy — clearing these toxic aggregates — would predict neuroprotection across multiple neurodegenerative diseases. This chain is assembled from cross-domain inferences; no vault source demonstrates it in neuronal models of PD, HD, or tau pathology directly.

**Selective neuronal vulnerability pattern (💡 Speculative):**
Parkinson's disease selectively destroys dopaminergic neurons of the substantia nigra. Huntington's disease preferentially damages striatal medium spiny neurons. If SLC13A5 expression is particularly high in these selectively vulnerable populations, their dependence on extracellular citrate as a conditional metabolic support (Kumar-2021: NaCT matters most under hypoxia, glutamine deprivation, or zinc stress) would predict that normal aging-related NaCT decline selectively disadvantages these neurons. The Allen Brain Cell Atlas query for SLC13A5 in dopaminergic and striatal neuron clusters would be the first test.

**CSF citrate as a pan-neurodegenerative biomarker (❓ Uncertain — Hofling-2026):**
Hofling-2026 shows that CSF citric acid discriminates iNPH from AD/MCI/FTD with AUC 0.97. AD and FTD are not separated from each other by CSF citrate in that study. This suggests that CSF citrate is more a marker of iNPH-specific physiology than a pan-neurodegenerative discriminator. Whether any neurodegenerative disease has specifically altered CSF citrate — beyond the normal aging rise documented by Lin-2021 — is not established for PD, HD, or other synucleinopathies.

## Evidence basis

- Source 1: [[research/Ferreira-2026]] — turquoise module KEGG enrichment for AD/PD/HD; SLC13A5 temporal and regional expression.
- Source 2: [[research/Fan-2021]] — brain-specific mIndy KO; dietary-restriction mimicry; cognitive benefit; neuroprotective framing.
- Source 3: [[research/Kopel-2021]] — INDY longevity biology review; caloric restriction connection; species-capacity caveat.
- Source 4: [[research/Birkenfeld-2011]] — AMPK activation in NaCT-deficient hepatocytes; mechanistic starting point for the AMPK-mTOR chain.
- Source 5: [[research/Hofling-2026]] — CSF citric acid as iNPH discriminator; AD/FTD/MCI do not separate.
- Source 6: AMPK-mTOR-autophagy in PD/HD context — No vault source. Cross-domain inference from established signaling literature. Requires primary literature verification.

## Connections to other nodes

- [[T2-MitochondrialBioenergetics]] — OXPHOS co-expression and AMPK-PGC1α are shared across AD and broader neurodegeneration contexts.
- [[T2-mTORSignaling]] — the mTOR-autophagy axis is the speculative neuroprotective mechanism potentially shared across protein-aggregation diseases.
- [[T1-INDYOrthologs]] — the evolutionary longevity biology is the conceptual backbone of the NaCT-neurodegeneration connection.
- [[T4-AlzheimerDisease]] — AD is the best-evidenced specific neurodegenerative connection; PD/HD are more speculative extensions of the same OXPHOS module argument.
- [[T4-MetabolicSyndrome]] — the longevity-metabolic axis connects metabolic syndrome protection and neurodegeneration protection as two faces of the same NaCT-AMPK-longevity mechanism.

## Open questions

1. In the Allen Brain Cell Atlas, is SLC13A5 expressed in dopaminergic (TH+) neurons of the substantia nigra — the selectively vulnerable cell type in PD?
2. In Slc13a5 KO mice, is there evidence of reduced MPTP-induced dopaminergic neuron loss, or improved rotarod performance in aged animals — a preclinical PD-relevant test?
3. Does the Ferreira-2026 turquoise module eigengene decline in publicly available transcriptomic datasets for PD or HD brain — testing whether the KEGG enrichment reflects actual gene expression changes in these diseases?
4. Does mTORC1 suppression (measurable by phospho-S6K1 in iPSC-derived neurons) occur in SLC13A5-deficient neurons, and does this correlate with increased autophagic flux — the direct test of the autophagy-neuroprotection chain?
5. Is there a common variant SLC13A5 genetic modifier signal in PD or HD GWAS datasets — testing whether common NaCT function variation modifies disease risk beyond AD?
