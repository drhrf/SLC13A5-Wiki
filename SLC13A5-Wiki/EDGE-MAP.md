---
tags: [slc13a5-wiki, synthesis, edge-map, network, connections, gaps]
node_type: synthesis
last_updated: 2026-05-10
---

# SLC13A5 Wiki — Edge Map

This document catalogs the connections between wiki nodes. Each edge is labeled with its epistemic status and the primary evidence source. The final section ranks the ten highest-priority connection gaps for future research.

---

## Confirmed edges (directly evidenced in vault sources)

### Tier 1 → Tier 2 edges

| From | To | Edge description | Evidence | Status |
|------|----|-----------------|----------|--------|
| T1-SLC13A5-Protein | T2-CitrateTCAIntegration | NaCT transports citrate 3:1 Na⁺:citrate³⁻; electrogenic; feeds cytoplasmic citrate pool | Kopel-2021; structural papers (7JSK/7JSJ) | ✅ |
| T1-SLC13A5-Protein | T2-HepaticLipidMetabolism | High-Vmax NaCT in hepatocytes feeds ACLY-derived lipogenesis | Birkenfeld-2011; Kopel-2021 | ✅ |
| T1-SLC13A5-Protein | T2-ZincCitrateInteraction | NaCT-imported citrate chelates extracellular zinc; reduces metal toxicity | Kumar-2021 | ✅ |
| T1-SLC13A5-GeneStructure | T2-TranscriptionalRegulation | PXR induces SLC13A5 in liver (not CAR); AhR also active; brain TF enrichment via TFAM/NRF-like | Li-2021-PXR; Ferreira-2026 | ✅ |
| T1-VariantCatalog | T2-CitrateTCAIntegration | All tested LoF variants converge on near-complete citrate transport loss | Klotz-2016; Jaramillo-Martinez-2024 | ✅ |
| T1-ExpressionAtlas | T2-MitochondrialBioenergetics | SLC13A5 in turquoise OXPHOS module; cerebrum declines postnatally | Ferreira-2026 | ✅ |
| T1-INDYOrthologs | T2-HepaticLipidMetabolism | mINDY KO metabolic protection recapitulates INDY longevity biology | Birkenfeld-2011; Willmes-2017 | ✅ |
| T1-INDYOrthologs | T2-mTORSignaling | mINDY KO AMPK activation → predicted mTORC1 suppression | Birkenfeld-2011; Fan-2021 | 🔶 |
| T1-InteractingProteins (ACLY) | T2-AcetylCoAProduction | ACLY cleaves citrate → oxaloacetate + acetyl-CoA; primary ACh synthesis source in cholinergic neurons | Gul-Hinc-2026 | ✅ |
| T1-InteractingProteins (ACSS2) | T2-AcetylCoAProduction | ACSS2 parallel acetate → nuclear acetyl-CoA; neuroprotective | Pourshafie-2026 | ✅ |
| T1-InteractingProteins (ZIP1) | T2-ZincCitrateInteraction | ZIP1 zinc uptake inhibits aconitase; cataplerosis in osteoblasts | Dirckx-2022 | ✅ |
| T1-InteractingProteins (SLC25A1) | T2-CitrateTCAIntegration | SLC25A1 exports mitochondrial citrate to cytoplasm; interplays with NaCT cytoplasmic pool | Dirckx-2022; mechanistic inference | ✅ |

### Tier 2 → Tier 2 edges

| From | To | Edge description | Evidence | Status |
|------|----|-----------------|----------|--------|
| T2-CitrateTCAIntegration | T2-AcetylCoAProduction | Cytoplasmic citrate → ACLY → acetyl-CoA; feeds both ACh synthesis and histone acetylation | Gul-Hinc-2026; Pourshafie-2026 | ✅ |
| T2-CitrateTCAIntegration | T2-GABAMetabolism | Citrate → isocitrate → α-KG → glutamate → GABA (TCA-derived GABA precursor) | Kopel-2021; mechanistic chain | 🔶 |
| T2-CitrateTCAIntegration | T2-NMDAModulation | Extracellular citrate chelates zinc → modulates NMDA receptor tone | Kumar-2021; zinc-citrate | 🔶 |
| T2-AcetylCoAProduction | T2-HistoneAcetylation | Cytoplasmic acetyl-CoA (from ACLY) enters nucleus → H3K27ac/H3K9ac at synaptic genes | Pourshafie-2026; cross-domain | 💡 |
| T2-HepaticLipidMetabolism | T2-MitochondrialBioenergetics | AMPK → PGC-1α → mitochondrial biogenesis; both activated by NaCT loss in hepatocytes | Birkenfeld-2011 | ✅ |
| T2-HepaticLipidMetabolism | T2-mTORSignaling | AMPK → TSC2 → Rheb → mTORC1 suppression; predicted secondary consequence of NaCT loss | Birkenfeld-2011 (AMPK); mTOR axis inference | 🔶 |
| T2-ZincCitrateInteraction | T2-NMDAModulation | Zinc modulates NMDA receptor activity; citrate buffering alters zinc availability for NMDA modulation | Cross-domain | 💡 |
| T2-Anaplerosis | T2-CitrateTCAIntegration | Alternative anaplerosis (glutamine, acetate, ketone bodies) compensates for absent NaCT-citrate | Kopel-2021; KD worsening context | 🔶 |
| T2-mTORSignaling | T2-MitochondrialBioenergetics | mTORC1 suppression → autophagy; AMPK → mitochondrial biogenesis; overlapping downstream effects | Established signaling | ✅ (in general) / 💡 (in NaCT context) |
| T2-TranscriptionalRegulation | T2-HepaticLipidMetabolism | PXR induction of SLC13A5 in liver → increased citrate import → increased lipogenesis | Li-2021-PXR | ✅ |

### Tier 2 → Tier 3 edges

| From | To | Edge description | Evidence | Status |
|------|----|-----------------|----------|--------|
| T2-CitrateTCAIntegration | T3-UrinaryMetabolomicsSignature | NaCT loss → accumulation of citrate and TCA intermediates in plasma, urine, CSF | Bainbridge-2017 | ✅ |
| T2-CitrateTCAIntegration | T3-ToothEnamelHypoplasia | NaCT loss in osteoblasts/ameloblasts → ZIP1 cataplerosis → excess mineral citrate → enamel defects | Dirckx-2022 | ✅ |
| T2-GABAMetabolism | T3-NeonatalEpilepsy | Reduced GABA precursor flux → reduced inhibitory tone → neonatal seizure susceptibility | Kopel-2021; pharmacological response data | 🔶 |
| T2-NMDAModulation | T3-NeonatalEpilepsy | Zinc chelation by citrate modulates NMDA excitability; NaCT loss may alter zinc-NMDA balance | Cross-domain inference | 💡 |
| T2-AcetylCoAProduction | T3-IntellectualDisability | Reduced acetyl-CoA → reduced histone acetylation at synaptic genes → permanent epigenetic deficit in critical developmental window | Cross-domain; Pourshafie-2026 | 💡 |
| T2-HistoneAcetylation | T3-IntellectualDisability | Failure to establish H3K27ac at synaptic gene loci during critical window → irreversible cognitive impairment | Cross-domain inference | 💡 |
| T2-HepaticLipidMetabolism | T3-HepaticMetabolicPhenotype | Mouse KO metabolic protection predicts analogous hepatic phenotype in DEE25 | Birkenfeld-2011 (mouse) | 🔶 |
| T2-HepaticLipidMetabolism | T3-MovementAbnormalities | ACLY → acetyl-CoA → fatty acid synthesis is analogous to myelin lipid synthesis in oligodendrocytes | Mechanistic analogy; Rigby-2022 cited | 💡 |

### Tier 3 → Tier 4 edges

| From | To | Edge description | Evidence | Status |
|------|----|-----------------|----------|--------|
| T3-UrinaryMetabolomicsSignature | T4-AlzheimerDisease | CSF citrate rises with aging (Lin-2021); plasma citrate predicts pre-dementia cognitive decline (Tremblay-Franco-2024) | Lin-2021; Tremblay-Franco-2024 | 🔶 |
| T3-HepaticMetabolicPhenotype | T4-MetabolicSyndrome | DEE25 patients are the natural human experiment for complete NaCT loss in liver; hepatic phenotype unstudied | Brown-Nye-Porter-2021 (absence finding) | ❓ |

### Tier 2 → Tier 4 edges

| From | To | Edge description | Evidence | Status |
|------|----|-----------------|----------|--------|
| T2-AcetylCoAProduction | T4-AlzheimerDisease | ACLY → acetyl-CoA → ACh synthesis; cholinergic deficit is hallmark of AD | Gul-Hinc-2026 | ✅ (ACLY step); 💡 (NaCT upstream) |
| T2-MitochondrialBioenergetics | T4-AlzheimerDisease | OXPHOS module co-expression with SLC13A5; AD KEGG enrichment | Ferreira-2026 | 🔶 |
| T2-HepaticLipidMetabolism | T4-MetabolicSyndrome | AMPK-lipogenesis axis is the hepatic mechanism for metabolic disease protection | Birkenfeld-2011 | ✅ (mouse) |
| T2-mTORSignaling | T4-NeurodegenerationBroadly | mTORC1 suppression → autophagy → aggregate clearance in neurodegeneration | Cross-domain | 💡 |
| T2-CitrateTCAIntegration | T4-CancerMetabolism | Conditional NaCT activity under hypoxia/glutamine deprivation in HCC | Kumar-2021 | ✅ (cell model) |

---

## Inferred edges (mechanistically plausible, not directly demonstrated in vault)

| From | To | Inferred connection | Basis | Priority to test |
|------|----|--------------------|----- |-----------------|
| T1-ExpressionAtlas | T4-AlzheimerDisease | Cerebral SLC13A5 decline with aging → reduced NaCT in aged cholinergic neurons | Ferreira-2026 trajectory + Gul-Hinc-2026 ACLY-ACh | High |
| T2-HistoneAcetylation | T3-IntellectualDisability | Epigenetic programming failure during critical window → permanent cognitive architecture deficit | Pourshafie-2026 (ACSS2); cross-domain ACLY analogy | High |
| T2-mTORSignaling | T3-IntellectualDisability | mTORC1 suppression during synaptogenesis → impaired translation-dependent circuit formation | Cross-domain | Medium |
| T2-GABAMetabolism | T3-MovementAbnormalities | GABA shaping motor circuit excitability in spinal/cortical circuits | General neuroscience; not NaCT-specific | Low |
| T1-InteractingProteins | T3-MovementAbnormalities | SLC13A5 in oligodendrocytes → myelin lipid synthesis → white matter development | Rigby-2022 overexpression data; Dirckx-2022 OPC precedent | Medium |
| T3-ToothEnamelHypoplasia | T4-AlzheimerDisease | Dental phenotype as a lifetime biomarker of NaCT function level — indirect AD-risk proxy | Speculative extension | Low |

---

## Top 10 ranked connection gaps

These are the connections most critical to the scientific story where evidence is absent or minimal. Ranked by: (1) scientific impact of confirming/refuting the connection, (2) feasibility with current methods.

**Gap 1 — SLC13A5 expression in ChAT-positive cholinergic neurons (Allen Brain Cell Atlas)**
Connects: T1-ExpressionAtlas → T4-AlzheimerDisease. The single most important unanswered expression question. If absent in ChAT+ clusters, the cholinergic vulnerability hypothesis loses its expression-level support.

**Gap 2 — Histone acetylation changes in SLC13A5-deficient human neurons**
Connects: T2-HistoneAcetylation → T3-IntellectualDisability. No vault source demonstrates altered histone acetylation in NaCT-deficient neurons. CUT&RUN in patient-derived iPSC neurons would directly test the epigenetic hypothesis for cognitive irreversibility.

**Gap 3 — TCA perturbation panel normalization in gene therapy trials**
Connects: T3-UrinaryMetabolomicsSignature → T3-NeonatalEpilepsy. Does the five-metabolite panel (citrate, succinate, fumarate, malate, α-KG) normalize concordantly after AAV9-SLC13A5 treatment? The most important pharmacodynamic readout for clinical trials.

**Gap 4 — Hepatic phenotype in DEE25 patients**
Connects: T3-HepaticMetabolicPhenotype → T4-MetabolicSyndrome. DEE25 patients are the only human model of complete liver NaCT loss. Plasma lipid panels and liver MRI-PDFF in DEE25 patients would directly test the metabolic protection hypothesis in humans.

**Gap 5 — mTORC1 suppression in SLC13A5-deficient neurons**
Connects: T2-mTORSignaling → T3-IntellectualDisability / T4-NeurodegenerationBroadly. Phospho-S6K1 and phospho-4EBP1 in DEE25 iPSC neurons vs isogenic controls is a direct, technically accessible measurement.

**Gap 6 — BBB permeability of NaCT inhibitors (ETG-5773, BI01383298)**
Connects: T4-MetabolicSyndrome → T3-NeonatalEpilepsy / T4-AlzheimerDisease. Brain exposure of pharmacological NaCT inhibitors is the single most critical safety data gap for the therapeutic program.

**Gap 7 — SLC13A5 in oligodendrocyte precursor cells**
Connects: T1-ExpressionAtlas → T3-MovementAbnormalities. Allen Brain Cell Atlas OPC cluster query. If confirmed, would provide a primary mechanism for white matter abnormalities and motor impairment in DEE25.

**Gap 8 — Ferreira-2026 module eigengene in ROSMAP AD samples**
Connects: T2-MitochondrialBioenergetics → T4-AlzheimerDisease. Does the turquoise module degrade in AD brain? A directly computable test using ROSMAP RNA-seq.

**Gap 9 — Mendelian randomization: SLC13A5 DMS scores → AD risk**
Connects: T1-VariantCatalog → T4-AlzheimerDisease. Uses Wang-2025 DMS data as genetic instruments. Tests whether NaCT function causally modifies AD risk. Requires IGAP/GWAS summary statistics.

**Gap 10 — Bone mineral density in DEE25 patients**
Connects: T3-ToothEnamelHypoplasia → T1-ExpressionAtlas. DXA in DEE25 patients would determine whether the bone cortical thinning seen in KO mice is present in humans — extending the Dirckx-2022 mechanism beyond teeth to systemic bone.
