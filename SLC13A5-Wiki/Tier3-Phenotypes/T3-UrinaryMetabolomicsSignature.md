---
tags: [slc13a5-wiki, tier-3, phenotype, metabolomics, urine, plasma, CSF, biomarker, TCA, diagnostic]
tier: 3
node_type: phenotype
epistemic_status: established
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-CitrateTCAIntegration]]"
  - "[[T1-VariantCatalog]]"
  - "[[T3-NeonatalEpilepsy]]"
  - "[[T4-AlzheimerDisease]]"
hypothesis_seeds:
  - "The full TCA perturbation panel (citrate + succinate + fumarate + malate + α-KG across plasma, urine, CSF) could serve as a multi-analyte pharmacodynamic readout for gene therapy trials — all five metabolites should normalize concordantly if NaCT is functionally restored"
  - "Untargeted urine metabolomics in DEE25 patients on ASMs would reveal drug-specific metabolic perturbations superimposed on the NaCT-loss signature — potentially identifying metabolomic biomarkers of drug response"
open_questions:
  - "Does the complete TCA perturbation signature (all five metabolites elevated) normalize in DEE25 patients treated with AAV9-SLC13A5 gene therapy — the most important pharmacodynamic question for clinical trials?"
  - "Is the urinary citrate:creatinine ratio a reliable, clinically available test for DEE25 diagnostic screening — and what is its sensitivity/specificity relative to plasma organic acid testing?"
  - "Do DEE25 patients have urinary lipid or sphingolipid abnormalities (consistent with Milosavljevic-2022 mouse metabolomics) — and would these serve as biomarkers of secondary metabolic pathology?"
---

# Urinary and Biofluid Metabolomics Signature

## Core claim

Loss of NaCT-mediated citrate import produces a diagnostic metabolomic signature in all three biofluids: elevated citrate in plasma, urine, and CSF, with secondary elevation of multiple TCA intermediates (succinate, fumarate, malate, α-ketoglutarate). This is the biochemical fingerprint of DEE25, established in a 5-patient cohort, validated at population scale via blood citrate correlating with NaCT function in UK Biobank, and directly useful for diagnostic disambiguation of VUS. Additional metabolomic findings from the Slc13a5 KO mouse (lipid and sphingolipid perturbations) have not yet been systematically characterized in DEE25 patients. Sources: [[research/Bainbridge-2017]], [[research/Wang-2025]], [[research/Lal-2026]], [[research/Milosavljevic-2022]].

## Mechanism

**The primary biofluid signature (✅ Established — Bainbridge-2017):**
When NaCT cannot clear extracellular citrate, citrate accumulates in all compartments from which the transporter normally clears it:
- Plasma: elevated citrate (detected by standard clinical plasma organic acid testing)
- Urine: elevated citrate (urinary organic acid testing)
- CSF: elevated citrate and TCA intermediates

The elevation extends beyond citrate to four other TCA intermediates: succinate, fumarate, malate, and α-ketoglutarate. This is because: (1) intracellular citrate depletion reduces TCA cycle flux, leading to backup of upstream intermediates; (2) compensatory anaplerosis (glutamine → TCA) produces excess intermediates that cannot be processed at normal rates.

The five-metabolite panel provides both diagnostic confirmation and mechanistic information: the full panel is consistent with a proximal block (failed citrate import), not a single enzymatic defect at a specific TCA enzyme.

**Population-scale validation (✅ Established — Wang-2025):**
Deep mutational scanning functional scores for SLC13A5 variants negatively correlate with blood citrate in UK Biobank participants (r = −0.63 for alleles with minor allele count >25). This validates that the citrate biomarker tracks NaCT function across the full spectrum of human SLC13A5 variant effects, from LoF to neutral, in the general population.

**Diagnostic utility for VUS (✅ Established — Lal-2026):**
When genetic testing identifies a VUS, elevated citrate in plasma or CSF provides functional evidence of NaCT loss — enabling diagnosis without a definitively classified variant. This is one of few rare disease settings where a metabolic biomarker can functionally substitute for experimental variant characterization.

**CSF aging biomarker (✅ Established — Lin-2021):**
In 75 cognitively unimpaired adults (ages 20–92), CSF citrate rises continuously with age as part of a five-metabolite aging signature. This is directionally opposite to what would be expected if aging NaCT activity decreases (which should reduce citrate clearing and raise CSF citrate) — consistent with declining NaCT in aging brain causing extracellular citrate accumulation, parallel to the DEE25 mechanism but at a milder level.

**Mouse lipid metabolomics (🔶 Emerging — Milosavljevic-2022):**
Milosavljevic-2022 performed untargeted metabolomics of Slc13a5 KO mice and found prominent perturbations in lipid homeostasis: fatty acids, sphingolipids, lysophospholipids. These secondary lipid changes, presumably downstream of reduced citrate-derived acetyl-CoA availability for lipid synthesis, have not been characterized in DEE25 patient biofluids. This is an unstudied gap — if analogous lipid perturbations exist in human DEE25 biofluids, they would expand the biomarker panel and provide insight into secondary pathology.

## Evidence basis

- Source 1: [[research/Bainbridge-2017]] — full TCA perturbation panel in 5 DEE25 patients; foundational metabolomics paper; all five metabolites elevated in plasma, urine, and CSF.
- Source 2: [[research/Wang-2025]] — UK Biobank blood citrate vs. DMS functional score correlation (r = −0.63); population-scale validation of citrate as NaCT activity proxy.
- Source 3: [[research/Lal-2026]] — citrate as diagnostic biomarker for VUS disambiguation in DEE25.
- Source 4: [[research/Lin-2021]] — CSF citrate rises with normal aging; aging-biomarker context.
- Source 5: [[research/Milosavljevic-2022]] — Slc13a5 KO mouse untargeted metabolomics; lipid perturbations documented in mouse but not yet in human DEE25.

## Connections to other nodes

- [[T2-CitrateTCAIntegration]] — the TCA perturbation signature is the direct metabolic consequence of the pathway disruption described in this Tier 2 node.
- [[T1-VariantCatalog]] — citrate biomarker enables VUS disambiguation when DMS functional data is not available for a specific variant.
- [[T3-NeonatalEpilepsy]] — the metabolic signature is most useful for diagnosis in neonates presenting with early seizures; plasma citrate can guide genetic testing.
- [[T4-AlzheimerDisease]] — CSF and plasma citrate as biomarkers in aging and pre-dementia connects this Tier 3 node to the Tier 4 AD connection via the Lin-2021 and Tremblay-Franco-2024 data.

## Open questions

1. Does the complete TCA perturbation panel (all five metabolites — citrate, succinate, fumarate, malate, α-KG) normalize concordantly in DEE25 patients who receive AAV9-SLC13A5 gene therapy — establishing it as a multi-analyte pharmacodynamic readout? If only citrate normalizes while the other four persist, that would suggest secondary metabolic dysregulation beyond the primary citrate-import defect.
2. Is the urinary citrate:creatinine ratio a reliable, simple screening test — and what is the sensitivity and specificity of a clinically available urinary organic acid panel for DEE25 in neonates with early seizures?
3. Do DEE25 patient plasma or CSF samples show lipid perturbations analogous to those in Slc13a5 KO mice (sphingolipids, lysophospholipids) — and if so, do these correlate with white matter integrity or motor severity?
4. Is there a metabolomic signature that distinguishes DEE25-related elevated plasma citrate from other causes of citric aciduria (renal tubular acidosis, mitochondrial citrate carrier deficiency, citrate lyase deficiency) — ensuring specificity of the biomarker for SLC13A5 loss?
