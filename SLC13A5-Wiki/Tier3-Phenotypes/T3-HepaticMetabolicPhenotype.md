---
tags: [slc13a5-wiki, tier-3, phenotype, liver, hepatic, NAFLD, metabolic, understudied-gap]
tier: 3
node_type: phenotype
epistemic_status: emerging
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-HepaticLipidMetabolism]]"
  - "[[T2-TranscriptionalRegulation]]"
  - "[[T1-ExpressionAtlas]]"
  - "[[T4-MetabolicSyndrome]]"
hypothesis_seeds:
  - "DEE25 patients may have subclinical hepatic metabolic abnormalities — reduced hepatic steatosis predisposition and altered lipid profiles — because NaCT loss in liver reduces citrate-driven lipogenesis; this is the opposite of the neurological phenotype but follows the same metabolic logic"
  - "Phenobarbital use in DEE25 (via PXR-mediated SLC13A5 induction in liver) may paradoxically alter hepatic metabolism in patients who are constitutively deficient — worth monitoring in clinical follow-up"
open_questions:
  - "Do DEE25 patients have measurably lower plasma LDL-cholesterol, triglycerides, or VLDL relative to age-matched controls — consistent with reduced hepatic lipogenesis from NaCT loss?"
  - "Is liver histology or imaging (MRI-PDFF) normal or showing reduced hepatic fat in DEE25 patients across childhood and adolescence — directly testing the metabolic protection hypothesis in humans?"
  - "Is any liver phenotype in DEE25 obscured by the anti-seizure medication burden (particularly valproic acid, which has well-known hepatotoxic effects at high doses)?"
---

# Hepatic Metabolic Phenotype

## Core claim

SLC13A5 is the highest-expressed gene in human liver among all tissues (approximately 60 RPKM in adults), yet hepatic involvement in DEE25 is largely unstudied in patients. The mouse Slc13a5 KO produces dramatic metabolic hepatic protection — reduced steatosis, improved insulin sensitivity, lower body weight — mediated through AMPK activation downstream of reduced cytoplasmic citrate. In human DEE25 patients, the liver phenotype is documented only minimally: Brown-Nye-Porter-2021 found no consistent hepatic abnormality in their records-based cohort, but this was not a systematic liver study. The hepatic phenotype in DEE25 is a critical gap: it may be protective (mimicking the KO mouse metabolic phenotype), absent (because compensatory mechanisms are sufficient), or obscured by medication effects. Sources: [[research/Birkenfeld-2011]], [[research/Brown-Nye-Porter-2021]], [[research/Kopel-2021]], [[research/Li-Wang-2021]], [[genes/SLC13A5]].

## Mechanism

**Predicted hepatic phenotype based on mouse KO data (🔶 Emerging — predicted, not confirmed in human DEE25):**
In Slc13a5 KO mice (Birkenfeld-2011), loss of hepatic NaCT produces:
- ~90% reduction in citrate incorporation into sterols and fatty acids
- 10–17% lower body weight
- Dramatically reduced hepatic steatosis on high-fat diet
- Improved insulin sensitivity (hyperinsulinemic-euglycemic clamp: hepatic glucose production reduced 50%)
- AMPK activation → PGC-1α → mitochondrial biogenesis

If human DEE25 patients have a comparable hepatic phenotype (accounting for the human SLC13A5 high-capacity transporter), they might be expected to show reduced hepatic fat, lower plasma triglycerides, and potentially improved insulin sensitivity relative to age-matched controls. This prediction has not been tested systematically.

**What is documented in DEE25 patients (❓ Largely unknown):**
Brown-Nye-Porter-2021 (n=15, Ciitizen records-based) specifically examined non-neurologic phenotypes. The key finding: "Liver, renal, cardiac: largely single occurrences or absent — no consistent extra-neurologic organ phenotype outside GI and respiratory." This is the only systematic survey of hepatic phenotype in DEE25 and it found nothing unusual. However, this study did not include liver biochemistry panels, imaging (ultrasound, MRI-PDFF for fat quantification), or lipid profiles — so absence of documented liver disease in records does not rule out subclinical liver metabolic changes.

**Valproic acid confound:**
Valproic acid (VPA) — the most widely used ASM in DEE25 (22/30 patients in Ozlu-2025) — has well-documented hepatotoxic potential at high doses (mitochondrial toxicity, microvesicular steatosis, hyperammonemia). VPA is also a known inhibitor of fatty acid beta-oxidation. In DEE25 patients on VPA, any baseline metabolic hepatic protection from NaCT loss could be masked by VPA-induced hepatic effects. Disentangling these requires systematic imaging with careful ASM documentation.

**Hepatic SLC13A5 regulation — clinical interaction:**
PXR agonism by phenobarbital induces SLC13A5 in normal hepatocytes (Li-2021-PXR). In DEE25 patients on phenobarbital, this induction is biochemically irrelevant (the induced mRNA produces no functional protein). However, PXR activation by PB could alter hepatic lipid metabolism through other PXR-target genes (CYP3A4, UGT1A1, etc.), potentially confounding any metabolic liver phenotype assessment.

## Evidence basis

- Source 1: [[research/Birkenfeld-2011]] — mouse KO hepatic metabolic protection; the template for the expected human phenotype.
- Source 2: [[research/Brown-Nye-Porter-2021]] — only systematic non-neurologic survey; no consistent liver phenotype found, but not systematically studied.
- Source 3: [[research/Li-Wang-2021]] — hepatic SLC13A5 as highest-expressed tissue; regulatory overview; NAFLD connection.
- Source 4: [[research/Kopel-2021]] — citrate's role in hepatocyte metabolism; therapeutic rationale for NaCT inhibition in metabolic disease.
- Source 5: [[genes/SLC13A5]] — SLC13A5 highest expression in liver; adult RPKM ~60.

## Connections to other nodes

- [[T2-HepaticLipidMetabolism]] — the upstream mechanism that would produce the predicted hepatic protection phenotype in DEE25.
- [[T2-TranscriptionalRegulation]] — hepatic regulation by PXR and AhR is relevant to drug interactions in DEE25 patients on ASMs.
- [[T1-ExpressionAtlas]] — liver as highest-expressing tissue; the expression context for why hepatic phenotype should be present if human biology mirrors mouse.
- [[T4-MetabolicSyndrome]] — if DEE25 patients prove to have metabolic hepatic protection, this would be the first human evidence that SLC13A5 LoF confers metabolic benefit analogous to mouse KO data.

## Open questions

1. Do DEE25 patients have lower plasma LDL-C, triglycerides, or VLDL-C than age-matched controls without considering ASM effects — the simplest first test of metabolic protection?
2. Is hepatic fat fraction (MRI-PDFF or liver ultrasound echogenicity) measurably lower in DEE25 patients than in age-matched controls — the imaging-based test of the steatosis-protection hypothesis?
3. Do DEE25 patients on valproic acid who have liver biochemistry monitored (as recommended by VPA guidelines) show any consistent pattern — either protective (lower baseline transaminases for age, lower lipid fractions) or harmful (VPA-mediated hepatotoxicity superimposed on NaCT-deficient liver)?
4. Is there a clinically actionable implication if DEE25 patients have metabolic hepatic protection — for example, should NaCT inhibitors (being developed for metabolic disease) specifically avoid use in heterozygous DEE25 carriers who already have reduced hepatic NaCT activity?
