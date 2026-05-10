---
tags: [slc13a5-wiki, contested, contradiction, ketogenic-diet, mouse-human, acetazolamide, methodology]
node_type: contested-claims-register
last_updated: 2026-05-10
---

# Contested Claims Register

This file documents claims in the vault that are either internally contradicted by other sources, contradicted by widely-held assumptions in the field, or where the evidence base is insufficient to choose between competing interpretations. Contradictions are not resolved here — they are registered, sourced, and paired with the evidence that would resolve them.

---

## CC1 — Ketogenic diet worsens symptoms in DEE25 (Klotz-2016 vs. general epilepsy practice)

**The contradiction.** The ketogenic diet (KD) is a first-line adjunct for pharmacoresistant pediatric epilepsy in most epilepsy types. It is widely used empirically across developmental and epileptic encephalopathies. However, [[research/Klotz-2016]] specifically reports that ketogenic diet and fasting *worsened* symptoms in their DEE25 patient cohort. This directly contradicts the common-practice assumption that KD is broadly applicable in pediatric epileptic encephalopathies.

**Mechanism-level reasoning for worsening.** The mechanistic case for worsening is plausible. In DEE25, the primary metabolic deficit is absent or severely reduced citrate import via NaCT. Citrate is a key anaplerotic substrate that feeds the TCA cycle through ACLY-mediated entry. The ketogenic diet achieves its anti-epileptic effect partly through ketone bodies replacing glucose as the main energy substrate and providing alternative anaplerosis (acetoacetate → acetyl-CoA → TCA entry). However, the KD also drastically reduces carbohydrate and thus glucose-derived pyruvate → OAA → TCA entry. If neuronal survival in DEE25 depends on residual glucose-derived anaplerosis to compensate for absent citrate-derived anaplerosis, the KD could remove this compensatory flux and precipitate metabolic crisis. This reasoning is plausible but has not been directly tested with metabolic flux measurements.

**Files involved.** [[conditions/SLC13A5-deficiency]] ("Ketogenic diet. [[Klotz-2016]] reports worsening of symptoms with ketogenic diet and fasting, contradicting earlier reports."). [[research/Klotz-2016]] (primary source). [[Tier2-Pathways/T2-Anaplerosis]] (records the conflict in the anaplerosis node). [[Tier3-Phenotypes/T3-NeonatalEpilepsy]] (flags as a contraindication).

**Status of the claim in newer literature.** [[research/Matricardi-2020]] and [[research/Brown-Nye-Porter-2021]] do not systematically assess KD outcomes. The Klotz-2016 finding has neither been replicated nor refuted in subsequent literature available in this vault. The default clinical position — based on Klotz-2016 as the most specific DEE25 data available — is that KD should not be routinely used in DEE25 and should be used only with extreme caution and close metabolic monitoring if no alternatives exist.

**Evidence that would resolve it.** A prospective or retrospective cohort study of KD use in DEE25 patients with systematic outcome documentation (seizure frequency, neurological scores, biofluid metabolomics before and during KD) would resolve whether worsening is reproducible. Ideally: continuous EEG and citrate/TCA metabolite panels during a structured KD trial in at least 5 DEE25 patients.

**Epistemic label.** 🔶 Emerging (replicated in one cohort; no prospective trial; mechanistic plausibility supports the worsening direction but is unconfirmed).

---

## CC2 — Fan-2021 cognitive benefit vs. DEE25 catastrophic loss (apparent paradox, not a true contradiction but requires resolution)

**The apparent contradiction.** [[research/Fan-2021]] demonstrates that nervous-system-specific deletion of mIndy (the mouse Slc13a5 ortholog) in adult mice produces significantly *improved* spatial memory, recognition memory, and motor coordination — a dietary-restriction-mimetic cognitive benefit. [[conditions/SLC13A5-deficiency]] and the entire Tier 3 phenotype set document that SLC13A5 loss in humans is catastrophic in neurodevelopment: neonatal seizures, severe intellectual disability, no cognitive recovery. These observations appear to directly contradict each other: how can losing the same transporter be beneficial (mice, adult) and catastrophic (humans, neonatal)?

**The reconciling framework.** The vault's standing interpretation (from [[overview]] and [[Tier1-Molecular/T1-INDYOrthologs]]) is that this is a developmental-stage and species-capacity interaction, not a true biological contradiction:
1. *Developmental stage*: Fan-2021 deleted mIndy in adult mice. DEE25 is caused by congenital complete absence of NaCT during the critical perinatal window. Neonatal brain under NaCT loss faces fundamentally different metabolic demands (rapid synaptogenesis, myelination, circuit formation) than adult brain.
2. *Species capacity*: Human SLC13A5 is a high-capacity transporter; mouse Slc13a5 is a low-capacity transporter. Citrate flux through NaCT in human neonatal neurons may be orders of magnitude higher than in mouse — meaning the metabolic consequence of complete loss is far more severe in humans than in mice.
3. *Compensation available*: Adult mouse brain that loses mIndy can presumably compensate through ACSS2 (acetate → acetyl-CoA), ketone body utilization, or other anaplerotic pathways. Neonatal human neurons in a critical developmental window may not have those compensatory reserves.

**Why this matters for drug safety.** If the reconciliation is correct — NaCT reduction is beneficial from a high set-point in adults but harmful from a low set-point in neonates — then the NaCT inhibitors being developed for metabolic disease (ETG-5773, BI01383298, Zhang-2024 compound) could be harmful if they reach the CNS in children or in elderly populations whose cerebral NaCT is already age-declined.

**Evidence that would resolve it.** A dose-response experiment in aged mice (not young adult) testing partial vs. complete mIndy reduction for cognitive outcomes would directly test the U-shaped hypothesis. In humans: a MR study linking SLC13A5 DMS functional score to both cognitive outcome and age (testing whether the relationship is non-linear) would be the bioinformatic version of this test.

**Epistemic label.** 💡 Speculative (the reconciling framework is coherent but untested; the U-shaped NaCT-cognition hypothesis is speculative per [[queries/hypotheses-SLC13A5-dementia-Alzheimer]] H8).

---

## CC3 — Mouse metabolic protection magnitude vs. predicted human effect (species-capacity confound)

**The contradiction.** All mouse Slc13a5 KO metabolic protection data (Birkenfeld-2011, Willmes-2017, Fan-2021) use the low-capacity mouse transporter. Human SLC13A5 is a high-capacity transporter with a higher Vmax than mouse Slc13a5. The kinetics are documented in Birkenfeld-2011 and T1-INDYOrthologs: mouse mINDY Km = 49 µM, Vmax = 3,760 pmol/(mg·min); human NaCT Km = 0.16 mM, with markedly higher Vmax. The species difference is primarily in maximum transport rate (Vmax), not in affinity direction — mouse actually has higher citrate affinity (lower Km) than human, but human moves more citrate per unit time. The vault consistently notes this caveat, but the critical implication is that loss of the *high-Vmax* human transporter would produce a *larger* metabolic perturbation than loss of the *lower-Vmax* mouse transporter — in both directions. For metabolic benefits (hepatic lipogenesis reduction), the benefit might be larger in humans. For risks (neuronal citrate depletion, dental enamel defects), the harm might also be larger. The mouse KO underestimates metabolic consequences in both directions.

**Files involved.** [[Tier1-Molecular/T1-INDYOrthologs]] (Km comparison table). [[Tier2-Pathways/T2-HepaticLipidMetabolism]] (Birkenfeld-2011 data with caveat). [[overview]] (leading caveat in "central tension" section). [[Tier3-Phenotypes/T3-HepaticMetabolicPhenotype]] (caveat on predicting hepatic protection magnitude from mouse data).

**Evidence that would resolve it.** Direct measurement of NaCT transport kinetics in human hepatocytes (primary or iPSC-derived) under identical experimental conditions as mouse hepatocytes (Birkenfeld-2011) would quantify the Vmax difference and allow metabolic flux modeling to estimate whether the magnitude difference is 2× or 10×.

**Epistemic label.** ✅ Established (the species capacity difference is established by kinetic data; the implication for metabolic protection magnitude is 🔶 Emerging — acknowledged in the literature but not directly quantified in human hepatocytes).

---

## CC4 — Acetazolamide effectiveness: promising signal vs. very limited evidence base

**The apparent claim.** [[research/Klotz-2016]] reports that acetazolamide reduced seizures in 4 of 9 patients in their cohort. This is the only novel pharmacological finding in the vault — not a conventional GABA-system agent, not a standard ASM. It has attracted attention as a potentially disease-relevant pharmacology.

**The problem.** The evidence base is n=9 patients, single-center, retrospective, no controls, no blinding, no standardized outcome metric. The 4/9 who responded may represent responders within a heterogeneous patient set rather than a mechanistic effect of acetazolamide on NaCT-deficient epilepsy. Acetazolamide (a carbonic anhydrase inhibitor) has broad electrolyte and pH effects; its mechanism in DEE25 — if real — is unknown and may not be specific.

**Files involved.** [[conditions/SLC13A5-deficiency]] ("acetazolamide reduced seizures in 4 of 9 [[Klotz-2016]] patients — the only novel pharmacology hit"). [[Tier3-Phenotypes/T3-NeonatalEpilepsy]] (acetazolamide listed among agents with partial support).

**Evidence that would resolve it.** Prospective N-of-1 or multi-center open-label trial of acetazolamide in DEE25 with standardized seizure-frequency and EEG endpoints, ideally with CSF/plasma citrate as a pharmacodynamic readout. The TESS Research Foundation registry could facilitate recruitment.

**Epistemic label.** 🔶 Emerging (4/9 is a signal; mechanism is unclear; single study with no replication in available vault).

---

## CC5 — CSF citrate: elevated in aging (Lin-2021) vs. normal or elevated in AD (Hofling-2026 interpretation)

**The apparent contradiction.** [[research/Lin-2021]] shows CSF citrate rises continuously with age in cognitively unimpaired adults (ages 20–92). [[research/Hofling-2026]] reports that CSF citric acid is specifically reduced in iNPH relative to AD/MCI/FTD, implying that AD/MCI/FTD do not have reduced CSF citrate — and by interpretation, that AD/MCI/FTD may actually have elevated CSF citrate relative to the iNPH baseline. These findings are not necessarily contradictory (Lin-2021 measures age-related rise in normals; Hofling-2026 compares disease states), but the interpretation — that CSF citrate "declines" in AD — is not directly supported by the vault's evidence and could be misleading.

**Resolution.** The correct interpretation is: (1) CSF citrate rises with normal aging; (2) it is specifically reduced in iNPH relative to other neurological diseases including AD. This does not mean CSF citrate is reduced in AD compared to age-matched cognitively normal controls — that comparison is not made in the vault's sources. The reduction in iNPH may reflect iNPH-specific pathophysiology (altered CSF dynamics/flow) rather than a NaCT-related signal.

**Evidence that would resolve it.** A study directly comparing CSF citrate in: (a) cognitively normal aged controls, (b) MCI patients, (c) AD patients with controlled for age — ideally using the same CSF collection protocol as Lin-2021. If CSF citrate in AD cases equals or exceeds age-matched normals, then the Lin-2021 aging rise persists into AD and is not reversed by AD pathology.

**Epistemic label.** ❓ Unknown (the comparison that would resolve this — AD vs age-matched controls for CSF citrate — is not in the vault).

---

## Summary table

| Code | Contradiction | Primary source | Contradicted by | Resolution needed | Status |
|------|--------------|----------------|-----------------|-------------------|--------|
| CC1 | KD worsens DEE25 | Klotz-2016 | General epilepsy practice | Prospective KD trial in DEE25 | 🔶 Emerging |
| CC2 | Fan-2021 benefit vs. DEE25 loss | Fan-2021 | Matricardi-2020, deficiency literature | Aged-mouse dose-response + human MR | 💡 Speculative |
| CC3 | Mouse metabolic protection magnitude vs. humans | Birkenfeld-2011 | Kopel-2021 (species-capacity caveat) | Human hepatocyte kinetics | ✅/🔶 Mixed |
| CC4 | Acetazolamide signal | Klotz-2016 | Absence of replication | Prospective DEE25 trial | 🔶 Emerging |
| CC5 | CSF citrate in aging vs. AD | Lin-2021 | Hofling-2026 (iNPH comparison) | AD vs age-matched control CSF citrate study | ❓ Unknown |
