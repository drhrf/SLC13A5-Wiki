---
tags: [slc13a5-wiki, synthesis, hypotheses, testable, translational]
node_type: synthesis
last_updated: 2026-05-10
---

# SLC13A5 Wiki — Hypothesis Registry

Twelve testable hypotheses derived from the wiki's evidence base, organized into three tiers by epistemic risk. Each hypothesis is paired with the evidence chain that motivates it, the experimental test that would confirm or refute it, and the falsification criteria.

---

## Tier A — Conservative hypotheses (high prior probability; incremental advance)

These build directly on established findings with high likelihood of confirmation. Confirmation would be impactful but not transformative.

---

### A1 — The five-metabolite panel is a pharmacodynamic readout for gene therapy

**Statement.** AAV9-SLC13A5 gene therapy in Slc13a5 KO mice or in DEE25 patients will normalize the five-metabolite biofluid signature (plasma/urine/CSF citrate, succinate, fumarate, malate, α-ketoglutarate) concordantly, and the extent of normalization will correlate with the degree of epileptiform activity rescue.

**Evidence chain.** Bainbridge-2017 established the five-metabolite panel as DEE25's biochemical fingerprint in 5 patients. Bailey-2026 demonstrated AAV9/SLC13A5 rescue of EEG epileptiform activity and CSF citrate in Slc13a5 KO mice. The logical next step — whether all five TCA metabolites normalize together — is the critical pharmacodynamic question for upcoming clinical trials.

**Test.** Measure all five metabolites in plasma, urine, and CSF of treated DEE25 patients and Slc13a5 KO mice before and at 3, 6, 12 months post-AAV9-SLC13A5 dosing. Correlate normalization slope with EEG seizure burden.

**Falsification criteria.** If citrate normalizes but the other four metabolites persist at pre-treatment levels, it would suggest that secondary metabolic dysregulation is not reversed by NaCT restoration alone — implying additional therapeutic targets beyond NaCT reconstitution.

**Linked nodes.** [[T3-UrinaryMetabolomicsSignature]], [[T3-NeonatalEpilepsy]], [[T2-CitrateTCAIntegration]].

---

### A2 — Citrate biomarker enables VUS clinical reclassification

**Statement.** In patients with SLC13A5 VUS and clinical features of DEE25, elevated plasma or CSF citrate will correctly identify pathogenic variants with sensitivity and specificity sufficient to guide clinical diagnosis without awaiting functional variant characterization.

**Evidence chain.** Wang-2025 DMS functional scores correlate with blood citrate (r = −0.63 in UK Biobank). Lal-2026 demonstrates citrate as a diagnostic tool for VUS disambiguation in DEE25. The population-scale validation of citrate as a NaCT-activity proxy provides a strong basis for clinical utility.

**Test.** Prospective collection of plasma citrate in 20+ DEE25 patients with characterized variants (known pathogenic) and 10+ patients with VUS. Define sensitivity/specificity cutoffs; compare citrate to DMS-predicted functional score. Assess positive predictive value for VUS reclassification.

**Falsification criteria.** If patients with confirmed pathogenic variants and patients with benign VUS have overlapping plasma citrate distributions (AUC < 0.85), the biomarker lacks clinical specificity for VUS discrimination in the clinical range.

**Linked nodes.** [[T3-UrinaryMetabolomicsSignature]], [[T1-VariantCatalog]].

---

### A3 — Bone mineral density is reduced in DEE25 patients

**Statement.** DEE25 patients will have measurably lower DXA-measured bone mineral density in cortical bone compartments (total hip, femoral neck, lumbar spine) relative to age- and mobility-matched controls, paralleling the bone cortical thinning and mechanical weakness documented in Slc13a5 KO mice.

**Evidence chain.** Dirckx-2022 established the ZIP1 cataplerosis mechanism leading to excess mineral citrate and reduced bone cortical thickness and mechanical strength in KO mice. Micro-CT of DEE25 primary teeth confirms reduced enamel and dentin density in 5 children. By the same mechanism, osteoblasts throughout the skeleton should produce bone with abnormal citrate content and architecture.

**Test.** DXA scans in 10+ DEE25 patients stratified by ambulatory status (to control for disuse osteopenia). Compare Z-scores to age/sex norms and to ambulatory-matched controls with other epilepsy diagnoses.

**Falsification criteria.** If DEE25 patients' DXA Z-scores do not differ from ambulatory-matched epileptic controls after controlling for calcium/vitamin D supplementation and ambulatory status, the predicted bone phenotype from mouse data does not manifest at the DXA-detectable level in humans.

**Linked nodes.** [[T3-ToothEnamelHypoplasia]], [[T2-ZincCitrateInteraction]], [[T1-ExpressionAtlas]].

---

### A4 — Ketogenic diet worsening is reproducible and metabolically explicable

**Statement.** The Klotz-2016 observation that ketogenic diet worsens DEE25 symptoms will be replicated in a larger cohort, and metabolic monitoring during KD will show increased plasma TCA intermediate perturbation (worsening of the five-metabolite signature) relative to baseline — mechanistically consistent with KD removing residual glucose-derived anaplerosis that compensates for absent NaCT-citrate.

**Evidence chain.** Klotz-2016 reports KD worsening in their cohort. The mechanistic rationale (KD removes compensatory glucose-derived OAA → TCA entry, leaving NaCT-deficient neurons with no anaplerotic buffer) is developed in [[CONTESTED-CLAIMS.md]] CC1. Newer cohort data (Matricardi-2020, Brown-Nye-Porter-2021, Ozlu-2025) do not systematically assess KD outcomes.

**Test.** Retrospective survey of DEE25 patients who received KD, with standardized seizure-frequency outcome and biofluid metabolomics before and during KD where available. Target: ≥15 patients with KD data.

**Falsification criteria.** If KD response in DEE25 is heterogeneous (half worsen, half improve or are neutral), or if the worsening rate is indistinguishable from other epileptic encephalopathies on KD, then KD worsening is not a specific DEE25 feature.

**Linked nodes.** [[CONTESTED-CLAIMS]], [[T2-Anaplerosis]], [[T3-NeonatalEpilepsy]].

---

## Tier B — Intermediate hypotheses (moderate prior probability; significant scientific advance if confirmed)

---

### B1 — SLC13A5 is expressed in ChAT-positive neurons and co-declines with ACLY in AD

**Statement.** Single-cell RNA-seq (Allen Brain Cell Atlas) will identify SLC13A5 expression in ChAT-positive cholinergic neuronal clusters, and SEA-AD data will show that SLC13A5 and ACLY expression are co-reduced in excitatory or cholinergic neuron subtypes in AD cases beyond what OXPHOS module co-regulation alone predicts.

**Evidence chain.** Gul-Hinc-2026 establishes ACLY as the primary ACh acetyl-CoA source in cholinergic neurons. Ferreira-2026 places SLC13A5 in the OXPHOS module enriched for AD pathways. If SLC13A5 is expressed in ChAT+ neurons and co-declines with ACLY in AD, the molecular chain NaCT → citrate → ACLY → ACh synthesis is supported at the single-cell level in human AD tissue.

**Test.** Query Allen Brain Cell Atlas for SLC13A5 expression in ChAT+ neuronal clusters. In SEA-AD pseudobulk data: test SLC13A5 log2FC in AD vs control, controlling for OXPHOS module eigengene; test SLC13A5-ACLY co-expression correlation within cell types.

**Falsification criteria.** If SLC13A5 is not detected above background in ChAT+ neuronal clusters in the Allen Brain Cell Atlas, the cholinergic vulnerability hypothesis has no expression-level support. If SLC13A5 decline in SEA-AD is fully explained by OXPHOS module co-regulation, it is not an independent AD signal.

**Linked nodes.** [[T4-AlzheimerDisease]], [[T2-AcetylCoAProduction]], [[T1-ExpressionAtlas]].

---

### B2 — The Ferreira-2026 OXPHOS module eigengene declines in AD brain

**Statement.** The turquoise WGCNA module from Ferreira-2026 will show a significantly lower module eigengene in AD DLPFC samples (ROSMAP) relative to age-matched cognitively normal controls, and SLC13A5 expression will track this eigengene decline proportionately.

**Evidence chain.** Ferreira-2026 KEGG enrichment for AD pathways in the turquoise module is a co-expression-based prediction. Actual AD gene expression data (ROSMAP) would determine whether the module actually degrades in AD tissue — the difference between a spurious KEGG annotation and a biologically relevant signal.

**Test.** Compute turquoise module eigengene in ROSMAP DLPFC bulk RNA-seq (n~500 donors with known Braak/CERAD/cognitive status). Compare eigengene across cognitive strata. Test whether SLC13A5 tracks eigengene or diverges.

**Falsification criteria.** If the module eigengene does not differ between AD and cognitively normal ROSMAP donors (p > 0.05 after age correction), then the KEGG enrichment for AD pathways reflects pathway label overlap rather than actual AD-related co-expression module breakdown.

**Linked nodes.** [[T2-MitochondrialBioenergetics]], [[T4-AlzheimerDisease]].

---

### B3 — Histone acetylation is impaired in SLC13A5-deficient human neurons during the critical developmental window

**Statement.** Patient-derived iPSC neurons with SLC13A5 LoF variants will show reduced H3K27ac at synaptic gene loci (including SYN1, SHANK3, DLG4/PSD-95) at the developmentally equivalent postnatal week 1–2 stage, and this will not be fully rescued by exogenous acetate supplementation (ACSS2 route) but will require citrate supplementation (ACLY route).

**Evidence chain.** Pourshafie-2026 demonstrates ACSS2-dependent nuclear acetyl-CoA → histone acetylation → neuroprotection in tau models. The nuclear acetyl-CoA pool has both ACLY (citrate-derived) and ACSS2 (acetate-derived) contributions. In NaCT-deficient neurons, the ACLY contribution is reduced. If histone acetylation at synaptic loci is impaired and not rescued by acetate alone, it would demonstrate that ACLY's citrate requirement — not ACSS2 — is the critical limiting node.

**Test.** CUT&RUN in DEE25 iPSC neurons (D60+ differentiation, postnatal-equivalent stage) for H3K27ac and H3K9ac at synaptic gene loci. Rescue experiment: citrate supplementation vs acetate supplementation vs combined.

**Falsification criteria.** If histone acetylation at synaptic loci does not differ from isogenic controls, or if acetate supplementation fully restores histone acetylation in NaCT-deficient neurons, then ACSS2 fully compensates for ACLY's citrate deficit and the epigenetic arm of the DEE25 hypothesis is not supported.

**Linked nodes.** [[T2-HistoneAcetylation]], [[T3-IntellectualDisability]], [[T2-AcetylCoAProduction]].

---

### B4 — Mendelian randomization supports a causal role of NaCT function in pre-dementia risk

**Statement.** Using Wang-2025 DMS functional scores as genetic instruments for plasma citrate, a two-sample Mendelian randomization will yield a significant causal estimate of plasma citrate on AD risk (from IGAP or FinnGen AD summary statistics), with direction consistent with higher citrate (lower NaCT function) predicting higher AD risk.

**Evidence chain.** Wang-2025 DMS scores validated as blood citrate instruments (r = −0.63 UK Biobank). Tremblay-Franco-2024 shows plasma citrate in TCA panel predicts cognitive decline in amyloid-positive subjects. MR requires valid instruments (met), exclusion restriction (citrate's effect on brain, not via other pathways — partially met), and relevance (met for common alleles).

**Test.** Standard two-sample MR using DMS-weighted SLC13A5 alleles as instruments. Sensitivity analyses: MR-Egger, weighted median, exclusion of pleiotropic alleles.

**Falsification criteria.** If MR estimates are null (IVW p > 0.05), or if sensitivity analyses suggest pervasive pleiotropy, the causal hypothesis for NaCT function → AD risk is not supported at the genetic level.

**Linked nodes.** [[T4-AlzheimerDisease]], [[T1-VariantCatalog]], [[T3-UrinaryMetabolomicsSignature]].

---

## Tier C — Radical hypotheses (low-to-moderate prior probability; transformative if confirmed)

---

### C1 — NaCT-cognition has a U-shaped relationship: the drug safety implication

**Statement.** The relationship between NaCT activity level and cognitive performance is non-linear (U-shaped): reduction from a high young-adult baseline (as in Fan-2021 young adult mice) is cognitively beneficial via DR mimicry; reduction from the already-low aged baseline crosses into the harmful range. In UK Biobank, SLC13A5 DMS functional score will show a non-monotone relationship with fluid intelligence — moderate-function alleles performing better than both high- and low-function extremes.

**Evidence chain.** Fan-2021 shows adult NaCT reduction improves cognition. Ferreira-2026 shows cerebral SLC13A5 continuously declines after the first postnatal year — aging may already reduce NaCT to a lower set-point. Lin-2021 CSF citrate rise with aging is consistent with reduced NaCT clearance. If NaCT is already in the "beneficial reduction" range in young adults but falls below threshold in the elderly, then pharmacological NaCT inhibitors could harm elderly patients.

**Test.** UK Biobank: plot DMS-weighted SLC13A5 genotype score vs fluid intelligence score. Fit both linear and quadratic models. Compare AIC. Stratify by age band (under 50 vs 50+ vs 65+) to test whether the relationship changes with age.

**Falsification criteria.** If the DMS score vs cognitive performance relationship is monotone linear (or null) across all age bands, the U-shaped hypothesis is not supported. A simple null — no relationship between SLC13A5 DMS score and cognition — would also fail to confirm it.

**Linked nodes.** [[CONTESTED-CLAIMS]] (CC2), [[T1-INDYOrthologs]], [[T4-AlzheimerDisease]], [[T4-MetabolicSyndrome]].

---

### C2 — Epigenetic memory of NaCT deficiency is irreversible after the critical window, even with gene therapy rescue

**Statement.** Gene therapy (AAV9-SLC13A5) administered after postnatal week 4 in Slc13a5 KO mice will normalize EEG, CSF citrate, and tooth enamel density in subsequently-formed teeth, but will NOT rescue cognitive performance (Barnes maze, novel object recognition) to wild-type levels — because histone acetylation at synaptic gene loci was not established during the critical epigenetic programming window and cannot be retroactively established by restoring citrate supply.

**Evidence chain.** Bailey-2026 shows both P10 and adult gene therapy rescue seizure phenotype and sleep architecture. It does not report cognitive outcome. Pourshafie-2026 demonstrates that ACSS2-dependent histone acetylation protects against tau-driven cognitive decline — with the implication that the critical window of acetylation establishment matters. If the epigenetic hypothesis is correct, seizure rescue and metabolic rescue should dissociate from cognitive rescue.

**Test.** Slc13a5 KO mice treated with AAV9-SLC13A5 at P10, P30, P60, or adult (6 months). Cognitive battery at 3 and 9 months post-treatment. CUT&RUN at synaptic gene loci in treated vs WT vs untreated KO. Expected: seizures rescued at all timepoints; cognition rescued only at P10 treatment; histone acetylation rescued only at P10 treatment.

**Falsification criteria.** If cognitive performance is equally rescued at P30 or P60 treatment as at P10 treatment, the critical-window epigenetic hypothesis is not supported. Alternatively, if P10-treated animals still have cognitive deficits despite normalized histone acetylation, then the cognitive impairment is not epigenetically mediated.

**Linked nodes.** [[T2-HistoneAcetylation]], [[T3-IntellectualDisability]], [[T3-NeonatalEpilepsy]].

---

### C3 — SLC13A5 is a dominantly acting dementia modifier through heterozygous NaCT hypofunction in aging

**Statement.** Heterozygous SLC13A5 LoF variants (haploinsufficient carriers who are neurologically normal but have ~50% NaCT activity from birth) will have measurably higher rates of age-related cognitive decline or earlier AD onset than non-carriers in population biobanks — because lifelong 50% NaCT haploinsufficiency progressively constrains the citrate supply available to aging cholinergic neurons, synergizing with Aβ-driven synaptic dysfunction to lower the clinical threshold for dementia.

**Evidence chain.** Wang-2025 DMS data establishes that heterozygous carriers of partially damaging SLC13A5 alleles have intermediate blood citrate (between WT and homozygous LoF). Tremblay-Franco-2024 TCA citrate panel predicts pre-dementia cognitive decline. The mechanistic chain from reduced NaCT activity → reduced ACh synthesis → cholinergic deficit → AD risk is established at each step but never directly in heterozygous human carriers.

**Test.** UK Biobank or ADSP: identify heterozygous SLC13A5 LoF variant carriers (predicted by DMS score < 0 or clinical LoF annotation). Compare incident dementia rates, MMSE trajectory, and fluid intelligence scores to non-carriers. Stratify by age (prediction: effect emerges after age 65 when aging-related NaCT decline interacts with haploinsufficiency).

**Falsification criteria.** If heterozygous SLC13A5 LoF carriers have no increased dementia rate or cognitive decline compared to matched non-carriers in UK Biobank, the dominantly-acting modifier hypothesis is not supported. A null finding here would substantially reduce the rationale for AD-prevention strategies targeting NaCT.

**Linked nodes.** [[T1-VariantCatalog]], [[T4-AlzheimerDisease]], [[T2-AcetylCoAProduction]].

---

### C4 — NaCT is the molecular link between metabolic syndrome and dementia risk: a shared mechanism

**Statement.** The epidemiological association between mid-life metabolic syndrome and late-life dementia risk is partially mediated by common SLC13A5 variant effects: individuals with high-functioning NaCT alleles have high hepatic citrate import → high lipogenesis → increased metabolic syndrome risk AND high neuronal citrate import → maintained cholinergic function → lower dementia risk. The allele that protects against metabolic syndrome (low NaCT function) is the same allele that increases cholinergic vulnerability in aging — creating a trade-off that partly explains why metabolic syndrome interventions do not fully prevent dementia.

**Evidence chain.** SLC13A5 is the highest-expressing gene in liver (metabolic role) and is expressed in brain cholinergic neurons (neurological role). Wang-2025 DMS score correlates with blood citrate across the full allelic spectrum. Willmes-2017 shows SLC13A5 upregulation in NAFLD/T2D. Gul-Hinc-2026 shows ACLY-ACh chain in cholinergic neurons. The trade-off hypothesis would explain why the same SLC13A5 genetic variation that protects the liver can potentially harm the brain.

**Test.** UK Biobank: quantify the SLC13A5 DMS score effect on hepatic steatosis/T2D risk AND cognitive performance/dementia risk simultaneously. Test whether the same alleles that are protective for metabolic syndrome are harmful for cognitive performance. MR: instrument citrate to test causal effects on both metabolic syndrome endpoints and cognitive endpoints.

**Falsification criteria.** If there is no antagonistic pleiotropy (the same alleles that reduce metabolic syndrome risk do not reduce cognitive performance or increase dementia risk), the trade-off hypothesis fails. A null MR result for the cognition endpoint would also fail to support it.

**Linked nodes.** [[T4-MetabolicSyndrome]], [[T4-AlzheimerDisease]], [[T1-INDYOrthologs]], [[T2-HepaticLipidMetabolism]].

---

## Summary table

| ID | Tier | Statement | Key test | Linked gap |
|----|------|-----------|----------|------------|
| A1 | Conservative | Five-metabolite panel normalizes in gene therapy | AAV9 treated mice/patients: serial metabolomics | EDGE-MAP Gap 3 |
| A2 | Conservative | Citrate enables VUS reclassification | Prospective citrate + DMS vs clinical diagnosis | EDGE-MAP Gap 2 (partial) |
| A3 | Conservative | Bone mineral density reduced in DEE25 | DXA in 10+ patients | EDGE-MAP Gap 10 |
| A4 | Conservative | KD worsening is reproducible | Retrospective KD-outcome survey, ≥15 patients | CONTESTED-CLAIMS CC1 |
| B1 | Intermediate | SLC13A5 in ChAT+ neurons; co-declines with ACLY in AD | Allen Cell Atlas + SEA-AD | EDGE-MAP Gap 1 |
| B2 | Intermediate | OXPHOS module eigengene declines in AD brain | ROSMAP module eigengene | EDGE-MAP Gap 8 |
| B3 | Intermediate | Histone acetylation impaired in DEE25 iPSC neurons | CUT&RUN in patient neurons | EDGE-MAP Gap 2 |
| B4 | Intermediate | MR: NaCT function → AD risk | Two-sample MR with DMS instruments | EDGE-MAP Gap 9 |
| C1 | Radical | U-shaped NaCT-cognition: drug safety implication | UK Biobank DMS score vs fluid intelligence, quadratic | CONTESTED-CLAIMS CC2 |
| C2 | Radical | Epigenetic memory irreversible after critical window | Bailey-2026 KO model + cognitive battery + CUT&RUN | EDGE-MAP Gap 2 |
| C3 | Radical | Heterozygous SLC13A5 LoF is a dementia modifier | UK Biobank or ADSP incident dementia in carriers | EDGE-MAP Gap 9 |
| C4 | Radical | SLC13A5 is the metabolic syndrome–dementia link | UK Biobank antagonistic pleiotropy analysis | EDGE-MAP Gap 1, 4 |
