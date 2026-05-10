---
tags: [slc13a5-wiki, tier-4, disease, metabolic-syndrome, NAFLD, T2D, obesity, INDY, longevity, hepatic, inhibitor]
tier: 4
node_type: disease-connection
epistemic_status: established-in-mouse-emerging-in-human
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-HepaticLipidMetabolism]]"
  - "[[T1-INDYOrthologs]]"
  - "[[T3-HepaticMetabolicPhenotype]]"
  - "[[T4-NeurodegenerationBroadly]]"
hypothesis_seeds:
  - "Hepatic SLC13A5 activity is a metabolic rheostat — patients with high-expression SLC13A5 haplotypes are more susceptible to diet-induced fatty liver and insulin resistance, while those with lower-expression haplotypes are partially protected — testable in UK Biobank with hepatic steatosis imaging and SLC13A5 DMS functional scores"
  - "ETG-5773 or BI01383298 hepatic NaCT inhibition will reduce steatosis and improve insulin sensitivity in humans with NAFLD without CNS effects, provided the BBB partition is verified — the first clinical test of the therapeutic hypothesis"
open_questions:
  - "Is hepatic SLC13A5 expression directly correlated with hepatic triglyceride content in human liver biopsies from non-alcoholic fatty liver disease cohorts — the most direct human translational test of the Birkenfeld-2011 mechanism?"
  - "What is the brain exposure fraction of ETG-5773 and BI01383298 in non-human primates — the safety-critical measurement before any human CNS-safety assumption can be made?"
  - "Do heterozygous SLC13A5 carriers in population biobanks have measurably lower rates of NAFLD, T2D, or obesity than wild-type — the epidemiological test of metabolic protection in loss-of-function human heterozygotes?"
---

# SLC13A5 and Metabolic Syndrome

## Core claim

SLC13A5/NaCT is a validated genetic and pharmacological target for metabolic disease protection in mouse models, with emerging human translational evidence. Loss of hepatic NaCT function in Slc13a5 KO mice produces comprehensive metabolic protection: reduced steatosis, improved insulin sensitivity, lower body weight, reduced plasma lipids — all mimicking the effects of caloric restriction. Human evidence includes upregulated hepatic SLC13A5 mRNA in obese T2D/NAFLD patients (Willmes-2017), population-scale citrate-NaCT correlation in UK Biobank (Wang-2025), and a pharmacological tool compound (ETG-5773, Zahn-2022; BI01383298, Quigley-2026) that recapitulates genetic KO metabolic effects in diet-induced obese mice. The therapeutic program is built on the hypothesis that hepatic NaCT inhibition — if BBB-impermeable — delivers metabolic benefit without neurological risk. Sources: [[research/Birkenfeld-2011]], [[research/Willmes-2017]], [[research/Zahn-2022]], [[research/Quigley-2026]], [[research/Kopel-2021]], [[research/Kopel-2020]], [[research/Wang-2025]].

## Mechanism

**Mouse KO metabolic phenotype (✅ Established — Birkenfeld-2011, Willmes-2017):**
Slc13a5 KO mice on chow or high-fat diet show:
- Body weight 10–17% lower than WT; fat mass reduced; lean mass preserved
- ¹⁴C-citrate incorporation into sterols and fatty acids reduced ~90% in KO hepatocytes
- Hepatic steatosis markedly reduced on HFD; triglyceride content and DAG content reduced 40–90%
- Basal plasma glucose and insulin reduced; insulin sensitivity improved on clamp
- Hepatic glucose production reduced 50%; peripheral glucose uptake increased 38%
- AMPK activation → PGC-1α → mitochondrial biogenesis → increased fatty acid oxidation
- SREBP-1c transcription reduced → downstream lipogenic enzymes reduced

The mechanistic cascade: NaCT loss → reduced cytoplasmic citrate → reduced ACLY activity → reduced acetyl-CoA for lipogenesis → reduced fatty acid and cholesterol synthesis. Simultaneously: reduced citrate-derived allosteric inhibition of PFK → increased glycolysis → alternative energy pathway engaged; reduced ATP/ADP ratio → AMPK activation → metabolic reprogramming.

**Human hepatic SLC13A5 upregulation in disease (🔶 Emerging — Willmes-2017):**
Hepatic SLC13A5 mRNA is significantly elevated in obese patients with T2D and NAFLD relative to lean controls. This is observational and cross-sectional — the causal direction (high SLC13A5 causes NAFLD, or NAFLD upregulates SLC13A5) is not established. However, it is the most direct human evidence that SLC13A5 expression tracks the disease state the transporter is proposed to drive.

**Metformin mechanism (🔶 Emerging — Kopel-2020):**
Kopel-2020 identifies SLC13A5/NaCT as a direct molecular target of metformin in hepatocytes. Metformin-mediated NaCT inhibition reduces intracellular citrate → reduced ACLY activity → reduced lipogenesis, complementing metformin's established complex I inhibition mechanism. This has safety implications: heterozygous DEE25 carriers on metformin already have ~50% NaCT activity; metformin could further reduce hepatic NaCT function to neurologically relevant levels.

**Pharmacological NaCT inhibition (🔶 Emerging — Zahn-2022, Quigley-2026, Zhang-2024):**
- *ETG-5773 (Zahn-2022)*: non-competitive, cross-species active NaCT inhibitor. In DIO mice: reduces hepatic steatosis, improves metabolic parameters. First pharmacological (not genetic) proof-of-concept for NaCT inhibition as a therapeutic strategy.
- *BI01383298 (Quigley-2026)*: IC₅₀ = 25 nM; >1,000-fold selective vs NaDC1/3; SGC chemical probe. Enables mechanistic studies without genetic KO.
- *Zhang-2024 compound*: IC₅₀ = 67 nM; described as the highest-potency NaCT inhibitor in the vault.

**The BBB safety partition (❓ Critical gap):**
All pharmacological development rests on the assumption that NaCT inhibitors that cannot cross the blood-brain barrier can deliver hepatic metabolic benefit without neurological harm. Brain permeability of ETG-5773, BI01383298, and Zhang-2024 compound is not documented in the available vault. Compound 2 (Huard-2015, the earlier Pfizer tool compound) brain exposure is also not stated. This is the single most critical safety-relevant gap in the metabolic-disease therapeutic program.

**Population-scale validation (✅ Established — Wang-2025):**
DMS functional scores for SLC13A5 variants negatively correlate with blood citrate in UK Biobank (r = −0.63). This validates that genetically-determined variation in NaCT function is measurable as plasma citrate in the general population — enabling epidemiological and MR studies of SLC13A5-mediated metabolic effects in humans.

**INDY longevity biology context (✅ Established for Drosophila; 🔶 Emerging for mammals):**
Drosophila INDY (I'm Not Dead Yet) partial loss-of-function extends median lifespan 30–50% by mimicking caloric restriction. C. elegans indy-1 loss similarly extends lifespan. Mouse mIndy KO recapitulates the caloric-restriction metabolic phenotype. The framing of SLC13A5 as a "longevity gene" in metabolic disease derives from this evolutionary conservation. Human evidence for the longevity connection is indirect: Willmes-2017 human liver expression data and Wang-2025 population-scale citrate correlation are both consistent but not directly causal.

## Evidence basis

- Source 1: [[research/Birkenfeld-2011]] — mouse KO metabolic phenotype; AMPK cascade; hepatocyte ¹⁴C-citrate lipogenesis reduction; insulin sensitivity.
- Source 2: [[research/Willmes-2017]] — human hepatic SLC13A5 upregulation in T2D/NAFLD; HFD mouse metabolic protection; inhibitor landscape review.
- Source 3: [[research/Kopel-2021]] — comprehensive review of the therapeutic rationale; species-capacity caveat; BBB partition rationale.
- Source 4: [[research/Kopel-2020]] — metformin as NaCT inhibitor; hepatocyte molecular mechanism.
- Source 5: [[research/Zahn-2022]] — ETG-5773 in DIO mice; pharmacological confirmation.
- Source 6: [[research/Quigley-2026]] — BI01383298 SGC probe; selectivity data.
- Source 7: [[research/Wang-2025]] — DMS scores; UK Biobank citrate-NaCT correlation.
- Source 8: [[research/Huard-2015]] — compound 2 (Pfizer NaCT inhibitor); competitive kinetics; in vivo endpoints.

## Connections to other nodes

- [[T2-HepaticLipidMetabolism]] — the AMPK-PGC1α-lipogenesis cascade is the central mechanism; this Tier 4 node is the disease-level consequence.
- [[T1-INDYOrthologs]] — the INDY longevity biology provides the evolutionary framework for why reducing NaCT activity is metabolically beneficial.
- [[T3-HepaticMetabolicPhenotype]] — DEE25 patients with congenital NaCT deficiency are the "experiment" in humans, but the hepatic phenotype in DEE25 is understudied.
- [[T4-NeurodegenerationBroadly]] — the longevity-metabolic axis connects metabolic syndrome protection to the broader aging and neurodegeneration connection.

## Open questions

1. Is hepatic SLC13A5 mRNA level directly correlated with hepatic triglyceride content in human liver biopsies from NAFLD cohorts — the most direct test of the Birkenfeld-2011 mechanism in humans?
2. What is the CNS bioavailability of ETG-5773 and BI01383298 in primates — the single most safety-critical measurement for the therapeutic program?
3. Do heterozygous SLC13A5 LoF carriers in UK Biobank have measurably lower rates of NAFLD, T2D, or higher BMI-adjusted lean mass — the epidemiological test of metabolic protection in haploinsufficient humans?
4. Does full or near-complete SLC13A5 loss in human liver (as in DEE25 patients) produce the same metabolic protection as Slc13a5 KO mice — specifically lower LDL-C, lower triglycerides, and reduced hepatic fat — and is this measurable in the existing patient records?
5. How does the species-capacity difference (mouse = low-capacity, human = high-capacity transporter) translate into quantitative predictions for the magnitude of metabolic benefit from NaCT inhibition in humans — and does the larger citrate flux in human liver mean the therapeutic effect will be proportionally larger?
