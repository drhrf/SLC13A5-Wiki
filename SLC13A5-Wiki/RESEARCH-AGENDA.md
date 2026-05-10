---
tags: [slc13a5-wiki, synthesis, research-agenda, priorities, timeline]
node_type: synthesis
last_updated: 2026-05-10
---

# SLC13A5 Wiki — Research Agenda

Prioritized research agenda organized across three time horizons. Priorities are assigned based on: (1) scientific impact if confirmed or refuted, (2) feasibility with current methods and resources, (3) clinical urgency (particularly for gene therapy support), and (4) dependency relationships (some questions must be answered before others become meaningful).

---

## Horizon 1 — 0 to 6 months (computational and publicly available datasets)

These can be executed with existing public data and computational tools. No new patient recruitment, wet lab work, or grant funding required beyond personnel time.

**H1.1 — Allen Brain Cell Atlas: SLC13A5 expression in neuronal subtypes**
Query the Allen Brain Cell Atlas single-cell RNA-seq data for SLC13A5 expression across all annotated neuronal clusters. Priority targets: ChAT+ (cholinergic), TH+ (dopaminergic), and GABAergic neuron clusters. Report: mean expression, percent cells expressing, and rank among all transporter genes. This directly tests the cholinergic vulnerability hypothesis (HYPOTHESES.md B1) and the motor/PD connection (T4-NeurodegenerationBroadly). Time estimate: 1 week.

**H1.2 — GTEx age regression: SLC13A5 in brain regions**
Extract SLC13A5 TPM from GTEx v8 or later across all brain regions. Fit age-regression models per region. Primary question: is the slope in frontal/temporal cortex significantly negative (cerebral decline confirmed in adults) and is the cerebellar slope positive (Ferreira-2026 trajectory in independent adult cohort)? Report slopes, confidence intervals, and regional ranking. Time estimate: 2 weeks.

**H1.3 — SEA-AD differential expression: SLC13A5 in AD vs control neurons**
Using the publicly available SEA-AD single-nucleus RNA-seq portal, perform pseudobulk differential expression analysis of SLC13A5 in excitatory neuron clusters (AD vs cognitively normal). Test independence from OXPHOS module co-regulation by including module eigengene as a covariate. Time estimate: 3 weeks (requires pseudobulk pipeline setup).

**H1.4 — ROSMAP module eigengene: Ferreira-2026 turquoise module in AD brain**
Obtain the turquoise module gene list from Ferreira-2026 supplementary data. Compute the module eigengene in ROSMAP DLPFC bulk RNA-seq (syn3388564) across Braak-stage strata. Does it decline monotonically with AD severity? Does SLC13A5 track the eigengene? Time estimate: 3 weeks (requires ROSMAP data access application).

**H1.5 — Contested-claims literature search: KD in DEE25**
Systematic PubMed/Embase search for all published DEE25 cohorts after 2016 reporting ketogenic diet outcomes. Extract KD responder/worsening data. Determine whether the Klotz-2016 worsening finding has been replicated or contradicted in subsequent literature not in the current vault. Time estimate: 1 week.

**H1.6 — OPC/oligodendrocyte SLC13A5 expression**
Query Allen Brain Cell Atlas for SLC13A5 in oligodendrocyte precursor cell (OPC) and mature oligodendrocyte clusters. If expressed, compute correlation with myelin-associated genes (MBP, PLP1, MAG). This directly tests the white matter hypothesis in T3-MovementAbnormalities. Time estimate: 1 week (concurrent with H1.1).

---

## Horizon 2 — 6 to 18 months (experimental biology and clinical data collection)

These require wet lab work, patient data collection, or data access applications for protected cohorts. Feasible within a 12-month experimental window with appropriate resources.

**H2.1 — CUT&RUN in DEE25 iPSC neurons: histone acetylation at synaptic loci**
Collaboration with a DEE25 iPSC biobank (TESS Research Foundation, Coriell, or patient-derived lines). Generate H3K27ac and H3K9ac CUT&RUN profiles in DEE25 iPSC neurons at D30 and D60 differentiation stages. Compare to isogenic CRISPR-corrected controls and variant-specific controls. Rescue experiment: citrate supplementation (1–5 mM) vs acetate supplementation (10 mM) vs combined. Expected duration: 9 months (iPSC differentiation + CUT&RUN + bioinformatic analysis). This directly tests HYPOTHESES.md B3 and provides the primary evidence for the epigenetic hypothesis of cognitive irreversibility.

**H2.2 — Bailey-2026 extension: cognitive phenotyping in gene-therapy-treated KO mice**
Extending the Bailey-2026 gene therapy experiment to include cognitive behavioral testing (Barnes maze, novel object recognition, fear conditioning) at 3 and 9 months post-treatment. Compare P10, P30, and adult treatment groups. CUT&RUN at synaptic loci in treated brains. This directly tests HYPOTHESES.md C2 (the irreversibility hypothesis) and has immediate implications for the clinical development program's expectations for cognitive outcomes. Expected duration: 12 months.

**H2.3 — DEE25 patient plasma lipid and liver imaging study**
Prospective collection of fasting lipid panels (LDL-C, HDL-C, total cholesterol, triglycerides, VLDL-C), liver transaminases, and liver MRI-PDFF (fat quantification) in ≥15 DEE25 patients, carefully stratified by ASM type (particularly separating VPA-exposed from VPA-naive). Compare to age-matched epilepsy controls on comparable ASMs. This tests T3-HepaticMetabolicPhenotype and HYPOTHESES.md A3 (bone) can be added as a DXA co-measure. Expected duration: 12 months (depends on patient access via TESS Research Foundation network).

**H2.4 — Five-metabolite panel in AAV9-SLC13A5-treated Slc13a5 KO mice**
Extending Bailey-2026 to measure all five TCA metabolites (plasma, urine, CSF) at baseline and 3, 6, 12 months post-treatment. Tests HYPOTHESES.md A1 and establishes the pharmacodynamic assay panel for clinical trials. Expected duration: 12 months (can run in parallel with H2.2).

**H2.5 — ETG-5773 and BI01383298 brain exposure in rodents**
PK/PD study measuring CNS concentration of ETG-5773 and BI01383298 after systemic dosing in rats or mice. Measure brain/plasma ratio at 1, 4, 8, and 24 hours post-dose. This is the most safety-critical measurement for the metabolic-disease therapeutic program. If brain exposure is significant, CNS safety testing (neurological function, EEG in WT mice on chronic dosing) is required before human trials. Expected duration: 6 months. Partner: medicinal chemistry/ADME group.

**H2.6 — Acetazolamide prospective pilot in DEE25**
N-of-5 prospective open-label pilot of acetazolamide in DEE25 patients with ongoing seizures, with standardized EEG, seizure diary, and CSF/plasma citrate monitoring before and during treatment. Primary outcome: ≥50% reduction in seizure frequency. This tests HYPOTHESES.md CC4 and could identify a disease-relevant treatment worth pursuing in a controlled trial. Expected duration: 6 months per patient; n=5 total ≈ 18 months for enrollment and data collection.

---

## Horizon 3 — 18+ months (clinical trials, genetic epidemiology, and advanced mechanistic work)

These require multi-year timelines, substantial funding, or large-scale genetic datasets.

**H3.1 — Phase I/II DEE25 gene therapy trial: metabolomics and cognitive endpoints**
The emerging gene therapy program (Bailey-2026 foundation) will require clinical-grade manufacturing, regulatory pathway, and patient recruitment. The research agenda contribution: ensure that the five-metabolite biofluid panel (HYPOTHESES.md A1), EEG seizure burden, sleep architecture, and cognitive battery (Vineland Adaptive Behavior Scales, Bayley, or BSID-IV for youngest patients) are all pre-specified in the trial design. The metabolomics endpoint from H2.4 should be validated before the trial opens. Expected timeline: IND filing 2028–2029 based on current program trajectory.

**H3.2 — Mendelian randomization: SLC13A5 DMS scores → AD risk**
Using the Wang-2025 DMS functional scores as genetic instruments for plasma citrate, perform two-sample MR against IGAP, FinnGen, or UK Biobank AD GWAS summary statistics. Sensitivity analyses for pleiotropy. This tests HYPOTHESES.md B4. Requires GWAS summary statistics access and collaboration with a statistical genetics group. Expected duration: 6 months computation after data access.

**H3.3 — UK Biobank: SLC13A5 DMS score vs cognition, linear vs U-shaped**
Requires UK Biobank data access application. Apply DMS functional scores to imputed genotype data. Outcome: fluid intelligence score, reaction time, digit span, incident dementia (longitudinal follow-up). Primary statistical test: linear vs quadratic fit to DMS score-cognition relationship. Age-stratified analysis. Expected duration: 18 months from data access to publication.

**H3.4 — ADSP/UK Biobank: heterozygous SLC13A5 LoF carrier dementia risk**
Identify heterozygous SLC13A5 LoF variant carriers in ADSP or UK Biobank. Compare incident dementia rates and cognitive trajectory to matched non-carriers. This tests HYPOTHESES.md C3. Requires large sample size (estimated: need >50 heterozygous LoF carriers for adequate power). Expected timeline: 18 months for data acquisition + analysis.

**H3.5 — Controlled acetazolamide trial in DEE25**
Building on H2.6, if the pilot is positive (≥3/5 responders), design a multi-center crossover trial with washout periods, standardized seizure diary, and EEG primary endpoint. This is the only novel pharmacological hypothesis in DEE25 that has even preliminary clinical support.

---

## Manuscript opportunities arising from this agenda

| Opportunity | Type | Key evidence needed | Timeline |
|-------------|------|---------------------|----------|
| Perspective: SLC13A5 as a node bridging metabolic disease and neurodegeneration | Perspective (no new data) | Wiki synthesis + public dataset queries H1.1-H1.4 | 6 months |
| Research article: Allen Brain Cell Atlas characterization of SLC13A5 in neuronal subtypes | Bioinformatics | H1.1, H1.6 | 3 months |
| Research article: Histone acetylation in DEE25 iPSC neurons | Experimental biology | H2.1 | 18 months |
| Clinical article: Hepatic metabolic phenotype in DEE25 patients | Clinical | H2.3 | 24 months |
| Research article: Five-metabolite pharmacodynamic readout in gene therapy | Translational | H2.4 | 18 months |

The perspective manuscript requires no new data and is directly supported by the wiki's current evidence synthesis. It is the near-term publication opportunity and the basis for the MANUSCRIPT-DRAFT.md.
