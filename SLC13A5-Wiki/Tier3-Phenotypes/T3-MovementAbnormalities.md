---
tags: [slc13a5-wiki, tier-3, phenotype, motor, hypotonia, spastic-quadriplegia, movement]
tier: 3
node_type: phenotype
epistemic_status: emerging
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-HepaticLipidMetabolism]]"
  - "[[T3-NeonatalEpilepsy]]"
  - "[[T3-IntellectualDisability]]"
hypothesis_seeds:
  - "Spastic quadriplegia reported in the Alsemari-2023 Saudi cohort may reflect an underascertained severe end of the motor phenotype spectrum, or may be specific to a founder variant with particularly complete NaCT loss in corticospinal circuits"
  - "Oligodendrocyte SLC13A5 expression during myelination contributes to corticospinal tract integrity — NaCT loss in OPCs/oligodendrocytes during the postnatal myelination surge impairs myelin lipid synthesis and white matter development"
open_questions:
  - "Is white matter integrity reduced in DEE25 patients on brain MRI — specifically in corticospinal tracts — and does this correlate with severity of motor impairment?"
  - "Is SLC13A5 expressed in oligodendrocyte precursor cells (OPCs) during the postnatal myelination peak — queryable in the Allen Brain Cell Atlas?"
  - "Does the spastic quadriplegia reported in Alsemari-2023 replicate in other DEE25 cohorts, or is it specific to the Saudi founder variants?"
---

# Movement Abnormalities

## Core claim

Diffuse hypotonia is present at onset in 86% of DEE25 patients and is the dominant early motor phenotype. Persistent motor delays affect virtually all patients. A Saudi Arabian cohort reported prominent spastic quadriplegia in 4 families — a motor phenotype not previously recognized as a defining feature, potentially representing the severe end of the motor spectrum or a variant-specific phenotype. Motor phenotype in DEE25 has been substantially under-characterized relative to epilepsy and intellectual disability. Sources: [[conditions/SLC13A5-deficiency]], [[research/Matricardi-2020]], [[research/Alsemari-2023]], [[research/Brown-Nye-Porter-2021]].

## Mechanism

**Established motor phenotype (✅):**
Diffuse hypotonia at onset is documented in 86% of patients (Matricardi-2020). The mechanism is presumed to be secondary to the encephalopathy: severe early neurological injury impairs motor circuit development. However, whether motor impairment is entirely secondary or has a primary metabolic component (direct NaCT loss in motor circuits or motor-projecting neurons) has not been tested.

**Motor trajectory:**
Persistent motor delays affect virtually all patients — none of the 14 Matricardi-2020 patients showed recovery of motor function commensurate with the recovery of seizure frequency. Brown-Nye-Porter-2021 (n=15, Ciitizen records-based) notes moderate GI burden and diverse respiratory complaints but does not characterize motor phenotype beyond the baseline encephalopathy severity. By adulthood (n=3 over 18 in Matricardi-2020), patients remain non-ambulatory or with significantly impaired ambulation.

**Spastic quadriplegia — Alsemari-2023 cohort (🔶 Emerging — single cohort, not yet replicated):**
Alsemari-2023 (Saudi Arabian cohort, 4 families) reported prominent spastic quadriplegia as a defining feature across their patients. Spastic quadriplegia implies corticospinal tract involvement. This extends the motor phenotype significantly — hypotonia and spasticity can co-exist in a child with encephalopathy (bilateral upper and lower motor neuron signs), but spastic quadriplegia as a prominent, consistent finding would suggest structural or functional corticospinal tract damage. Replication in other cohorts is needed. Possible explanations: (a) the Saudi founder variants produce a particularly severe phenotype at the severe end of the spectrum; (b) corticospinal tract involvement has been underreported elsewhere because standard neurological examination of severely encephalopathic neonates may not distinguish hypotonia from emerging spasticity; (c) a primary white matter component exists.

**White matter hypothesis (💡 Speculative):**
Neuron-specific SLC13A5 overexpression in mice produces disrupted white matter integrity (Rigby-2022, cited in vault). Dirckx-2022 establishes SLC13A5 expression in non-neuronal mineralizing cells — the precedent for non-neuronal SLC13A5 expression with functional consequences. If SLC13A5 is expressed in oligodendrocytes or OPCs during the postnatal myelination surge, NaCT loss could impair myelin lipid synthesis (citrate → ACLY → acetyl-CoA → fatty acid synthesis → myelin lipids), producing white matter pathology. This would provide a primary mechanism for motor impairment independent of the neuronal seizure-mediated damage story.

## Evidence basis

- Source 1: [[research/Matricardi-2020]] — diffuse hypotonia at onset 86%; persistent motor delays; baseline motor natural history.
- Source 2: [[research/Alsemari-2023]] — spastic quadriplegia in Saudi cohort; 4 families; motor phenotype extension.
- Source 3: [[research/Brown-Nye-Porter-2021]] — non-neurologic health outcomes; respiratory and GI burden; limited motor characterization.
- Source 4: [[conditions/SLC13A5-deficiency]] — integrated motor phenotype summary.
- Source 5: White matter / oligodendrocyte SLC13A5 expression — No vault source confirms OPC/oligodendrocyte expression directly. The myelination hypothesis is derived from the overexpression white matter finding (Rigby-2022, referenced in vault) and the DEE25 developmental disorder hypotheses file. Requires primary literature verification for the loss-of-function direction.

## Connections to other nodes

- [[T2-HepaticLipidMetabolism]] — the ACLY → acetyl-CoA → fatty acid synthesis pathway in liver is directly analogous to the hypothesized pathway in oligodendrocytes (myelin lipid synthesis); this Tier 2 node provides the metabolic framework.
- [[T3-NeonatalEpilepsy]] — motor impairment co-occurs with seizures; both are present at onset, but the mechanistic relationship is not established.
- [[T3-IntellectualDisability]] — motor and cognitive impairments co-occur and neither recovers with seizure remission; they share developmental trajectories but may have distinct primary mechanisms.

## Open questions

1. Is white matter integrity reduced in DEE25 patients on brain MRI quantitative diffusion tensor imaging (DTI) — and does fractional anisotropy in corticospinal tracts correlate with severity of motor impairment? This is directly measurable in existing or prospectively collected patient MRI data.
2. Does SLC13A5 expression appear in oligodendrocyte or OPC clusters in the Allen Brain Cell Atlas — the most direct test of the myelination hypothesis?
3. Does spastic quadriplegia in Alsemari-2023 associate with specific variant types (Class I vs. Class II, or specific founder alleles) — and is it present in patients from other cohorts at similar variant-severity levels when specifically assessed?
4. In Slc13a5 KO mice, is there evidence of white matter abnormalities on MRI or myelin staining — and does AAV9 gene therapy (Bailey-2026) normalize white matter structure if administered prenatally or in the neonatal period?
