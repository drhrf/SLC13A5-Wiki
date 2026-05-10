---
tags: [slc13a5-wiki, tier-2, pathway, acetyl-CoA, ACLY, ACSS2, histone-acetylation, epigenetics, neurodegeneration]
tier: 2
node_type: pathway
epistemic_status: emerging
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-CitrateTCAIntegration]]"
  - "[[T2-HistoneAcetylation]]"
  - "[[T2-GABAMetabolism]]"
  - "[[T1-InteractingProteins]]"
  - "[[T4-AlzheimerDisease]]"
  - "[[T4-NeurodegenerationBroadly]]"
hypothesis_seeds:
  - "ACLY and ACSS2 compete for nuclear acetyl-CoA demand in neurons — reduced ACLY substrate (citrate) from NaCT loss could upregulate ACSS2 as a compensatory response, partially buffering the epigenetic consequences"
  - "The cholinergic deficit in AD may be initiated upstream of neuron loss — by reduced citrate supply to ACLY in aging basal forebrain neurons, constraining ACh synthesis years before cell death"
open_questions:
  - "What fraction of nuclear acetyl-CoA in developing human cortical neurons comes from ACLY (citrate-derived) vs. ACSS2 (acetate-derived) — and does this fraction change during the first postnatal year when SLC13A5 expression is highest?"
  - "Is ACLY expression in cholinergic neurons of the basal forebrain selectively reduced in early-stage AD (Braak I-II) relative to other neuronal populations — supporting the hypothesis that the NaCT-ACLY-ACh axis is preferentially disrupted?"
  - "Does histone acetylation at synaptic gene loci in iPSC-derived neurons from DEE25 patients differ from isogenic controls — providing direct evidence for the epigenetic programming hypothesis?"
---

# Acetyl-CoA Production from Citrate

## Core claim

Cytoplasmic citrate, derived from NaCT-mediated import or SLC25A1-mediated mitochondrial export, is the primary substrate for ATP-citrate lyase (ACLY), which cleaves it into acetyl-CoA + oxaloacetate. In neurons, this acetyl-CoA serves two neuroprotective functions: acetylcholine synthesis in cholinergic neurons (directly demonstrated) and histone acetylation for neuroprotective gene regulation (demonstrated for ACSS2-derived acetyl-CoA; inferred for ACLY-derived). Both functions decline with aging and neurodegeneration. Sources: [[research/Gul-Hinc-2026]], [[research/Pourshafie-2026]], [[mechanisms/acetyl-CoA-neurodegeneration]].

## Mechanism

The pathway proceeds in two branches from ACLY-generated acetyl-CoA:

**Branch 1 — Acetylcholine synthesis (✅ Established):**
```
Extracellular citrate → NaCT → cytoplasmic citrate → ACLY → acetyl-CoA
acetyl-CoA + choline → ChAT → acetylcholine → synaptic release
```
Gul-Hinc-2026 demonstrated that ACLY is the *primary* source of acetyl-CoA for ACh synthesis in cholinergic neurons by isotope tracing (citrate-derived acetyl-CoA → ACh confirmed). Regional correlation between ACLY activity and ChAT activity was strong across multiple brain regions. ACLY is present at presynaptic cholinergic terminals, consistent with local acetyl-CoA provision at the site of ACh synthesis. This makes the citrate supply chain rate-limiting for ACh synthesis in cholinergic neurons — the same neurons that degenerate in AD.

**Branch 2 — Histone acetylation / epigenetic regulation (🔶 Emerging):**
```
Acetyl-CoA (from ACLY or ACSS2) → HAT (histone acetyltransferases) →
H3K9ac, H3K27ac at synaptic gene loci → neuroprotective gene expression
```
Pourshafie-2026 demonstrated that ACSS2-derived nuclear acetyl-CoA sustains histone acetylation at synaptic gene loci and protects neurons from tau-driven cognitive decline. Normal aging reduces nuclear ACSS2 activity → reduced histone acetylation → impaired synaptic gene regulation. ACLY provides a parallel route to the same nuclear pool from the citrate side. The fraction of nuclear acetyl-CoA from ACLY vs. ACSS2 in neurons is not established.

**Parallel route — ACSS2 (🔶 Emerging):**
```
Acetate → ACSS2 → nuclear acetyl-CoA → histone acetylation
```
ACSS2 operates independently of citrate. In conditions where citrate supply is reduced (NaCT loss, aging-related NaCT decline), ACSS2-derived acetyl-CoA could compensate for reduced ACLY flux. Whether this compensation is sufficient, partial, or saturated at the acetate concentrations available in aging brain is not known.

**The aging intersection:**
NaCT expression declines in human cerebrum after the first postnatal year (Ferreira-2026). If this decline is steep enough in late life, cytoplasmic citrate in neurons falls → reduced ACLY flux → reduced ACh synthesis capacity and/or reduced nuclear acetyl-CoA → epigenetic dysregulation of synaptic genes. These are mechanistically plausible consequences of an aging NaCT expression decline, not directly demonstrated in humans. The Fan-2021 finding (brain NaCT reduction *improves* cognition in *young adult* mice) complicates this — suggesting dose-dependency that may change with age.

## Evidence basis

- Source 1: [[research/Gul-Hinc-2026]] — ACLY as primary acetyl-CoA source for ACh; isotope tracing, regional ChAT-ACLY correlation, ACLY at presynaptic terminals. PMID 41596431.
- Source 2: [[research/Pourshafie-2026]] — ACSS2 → histone acetylation → neuroprotection from tau; normal aging reduces this; ACSS2 overexpression rescues. PMID 41512015.
- Source 3: [[mechanisms/acetyl-CoA-neurodegeneration]] — integrative synthesis of ACLY/ACSS2 roles in the neurodegeneration context; the full hypothesis chain.
- Source 4: [[research/Fan-2021]] — nervous-system mINDY KO improves cognition in adult mice; perturbational evidence that brain citrate reduction is not simply harmful in adults.
- Source 5: [[research/Ferreira-2026]] — cerebrum SLC13A5 expression peak-then-decline; context for the aging-driven NaCT expression change that would reduce ACLY substrate.

## Connections to other nodes

- [[T2-CitrateTCAIntegration]] — upstream; cytoplasmic citrate pool is the substrate source for ACLY; this node explains what happens to citrate once inside the cell.
- [[T2-HistoneAcetylation]] — downstream branch; nuclear acetyl-CoA from ACLY (or ACSS2) drives this pathway.
- [[T2-GABAMetabolism]] — parallel downstream; TCA cycle intermediates from citrate → α-KG → glutamate → GABA; competing pathway for the same citrate carbon.
- [[T1-InteractingProteins]] — ACLY and ACSS2 are the primary interacting proteins discussed here.
- [[T4-AlzheimerDisease]] — the cholinergic arm of this pathway directly connects to the AD disease mechanism; reduced ACh synthesis from reduced ACLY flux is the core mechanistic hypothesis.
- [[T4-NeurodegenerationBroadly]] — the histone acetylation arm connects to general epigenetic neuroprotection failure in aging.

## Open questions

1. In iPSC-derived cholinergic neurons from DEE25 patients (compared to isogenic controls with SLC13A5 restored), is ACh synthesis reduced — and is this reduction rescued by citrate supplementation or ACSS2 overexpression?
2. What is the quantitative partition between ACLY and ACSS2 for nuclear acetyl-CoA in mature human cortical neurons at different ages — and does this partition shift in AD tissue?
3. Does the Fan-2021 cognitive benefit from brain NaCT reduction in young adult mice come with any reduction in ACh synthesis or histone acetylation in cholinergic basal forebrain neurons — which would argue that the "benefit" is not from the ACLY arm but from a different mechanism (perhaps reduced lipid synthesis, reduced glutamate, or metabolic caloric-restriction effects)?
4. Can plasma or CSF ACLY activity levels serve as an accessible proxy for brain ACLY function — and would these levels be reduced in DEE25 patients relative to controls?
