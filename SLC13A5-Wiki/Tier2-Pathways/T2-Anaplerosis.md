---
tags: [slc13a5-wiki, tier-2, pathway, anaplerosis, glutamine, ketone-bodies, acetate, compensation, metabolic-flexibility]
tier: 2
node_type: pathway
epistemic_status: emerging
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-CitrateTCAIntegration]]"
  - "[[T2-GABAMetabolism]]"
  - "[[T2-HepaticLipidMetabolism]]"
  - "[[T3-NeonatalEpilepsy]]"
hypothesis_seeds:
  - "Glutamine supplementation could partially compensate for NaCT loss in DEE25 neurons by providing an alternative anaplerotic substrate for GABA synthesis — testable in iPSC neurons without requiring gene therapy"
  - "The worsening of symptoms with ketogenic diet in DEE25 (Klotz-2016) may reflect ketone bodies competing with citrate for metabolic pathways, further reducing the cytoplasmic citrate pool that NaCT-deficient neurons are already struggling to maintain"
open_questions:
  - "Does 13C-glutamine tracing in DEE25 iPSC neurons show increased glutamine-to-GABA flux relative to controls — indicating compensatory anaplerosis — or is this compensation pathway also impaired?"
  - "Why does ketogenic diet worsen DEE25 symptoms (Klotz-2016) — mechanistically, what does ketone body elevation do to the citrate pool or GABA synthesis in neurons lacking NaCT?"
  - "Is acetate supplementation (feeding ACSS2 as an ACLY bypass) beneficial in SLC13A5-deficient neurons — specifically for restoring nuclear acetyl-CoA and histone acetylation without requiring citrate transport?"
---

# Anaplerosis: Alternative Substrates for Citrate-Deficient Neurons

## Core claim

When NaCT-mediated citrate import is absent (DEE25), neurons must rely on alternative anaplerotic substrates to maintain TCA cycle intermediates, neurotransmitter precursor pools, and acetyl-CoA production. The primary candidates are glutamine, acetate, and (when available) ketone bodies. Evidence for the adequacy or inadequacy of this compensation in SLC13A5-deficient human neurons is indirect, but the worsening of symptoms with ketogenic diet (Klotz-2016) suggests that altered anaplerotic substrate availability can worsen rather than help the DEE25 metabolic state. Sources: [[research/Kopel-2021]], [[research/Kumar-2021]], [[research/Klotz-2016]], [[conditions/SLC13A5-deficiency]].

## Mechanism

**Anaplerotic substrate options:**

**1. Glutamine (🔶 Emerging as potential compensator):**
Glutamine → glutamate (via glutaminase) → α-KG (via GDH or transaminase) → TCA cycle entry. This provides both a GABA synthesis precursor (glutamate) and a TCA intermediate that can generate citrate via the cycle. Glutamine is the most abundant amino acid in plasma and CSF. In energy-stressed neurons, glutamine anaplerosis is upregulated. Whether it compensates adequately for NaCT loss in human neurons is not directly measured in the vault.

**2. Acetate (🔶 Emerging):**
Acetate → acetyl-CoA via ACSS2. This provides cytoplasmic and nuclear acetyl-CoA without requiring citrate as an intermediate, bypassing the NaCT-ACLY step. Pourshafie-2026 established ACSS2 as a neuroprotective acetyl-CoA source independent of ACLY. Supplemental acetate could in principle restore nuclear acetyl-CoA in NaCT-deficient neurons without restoring citrate transport. Whether acetate supplementation is sufficient to fully compensate for all downstream functions of NaCT (GABA synthesis, NMDA modulation, zinc buffering) is unknown.

**3. Ketone bodies (❓ Unclear — potentially counterproductive in DEE25):**
β-hydroxybutyrate → acetoacetate → acetyl-CoA; or → succinyl-CoA (an odd-carbon pathway). In most epilepsy forms, ketogenic diet (which elevates ketone bodies) is anticonvulsant. The mechanism includes increased GABA, reduced glutamate, and metabolic effects. In DEE25, ketogenic diet *worsened* symptoms in the Klotz-2016 cohort — a striking and unexplained exception. This is one of the vault's most important clinical conflicts. Possible mechanism: ketone body oxidation generates acetyl-CoA that does not substitute for citrate-derived substrates; alternatively, ketogenic state reduces glutamine availability (anaplerotic competitor) or alters the TCA balance in a way that is specifically harmful when citrate import is absent.

**4. Exogenous citrate supplementation (❓ Unknown efficacy):**
Administering citrate directly could in principle supply the substrate that NaCT would normally import. However, Kumar-2021 showed that in SLC13A5 KO cells, exogenous citrate cannot be utilized effectively because the transporter is absent — the cell cannot take it up via NaCT. Whether citrate crosses membranes through other routes (passive diffusion at very high concentrations, alternative transporters) in sufficient quantities to be therapeutic is not established.

**Elevated TCA intermediates as evidence of failed compensation:**
Bainbridge-2017 showed elevated citrate + succinate + fumarate + malate + α-KG in all biofluids of DEE25 patients. The elevation of multiple TCA intermediates (not just citrate) suggests the compensation is incomplete: the system is trying to maintain TCA flux through alternative routes but producing a metabolic spillover into the extracellular space rather than normal metabolic utilization.

## Evidence basis

- Source 1: [[research/Klotz-2016]] — ketogenic diet and fasting worsen symptoms in DEE25 cohort; critical clinical conflict.
- Source 2: [[research/Kumar-2021]] — conditional NaCT importance; anaplerosis via glutamine and citrate import distinguishable; exogenous citrate cannot substitute for NaCT-mediated import in KO cells.
- Source 3: [[research/Bainbridge-2017]] — full TCA perturbation signature; indirect evidence of inadequate anaplerotic compensation.
- Source 4: [[research/Pourshafie-2026]] — ACSS2 as acetate → acetyl-CoA route bypassing ACLY; potential compensation strategy for the acetyl-CoA deficit.
- Source 5: [[research/Kopel-2021]] — framing of anaplerosis in SLC13A5 deficiency context.

## Connections to other nodes

- [[T2-CitrateTCAIntegration]] — anaplerosis is the compensatory response to the primary TCA perturbation in this node.
- [[T2-GABAMetabolism]] — glutamine anaplerosis feeds the same glutamate pool used for GABA synthesis; glutamine could partially compensate for reduced citrate → α-KG → glutamate flux.
- [[T2-HepaticLipidMetabolism]] — in hepatocytes, ketone body metabolism and citrate-dependent lipogenesis compete; the ketogenic diet conflict in DEE25 may reflect hepatic metabolic changes spilling over into neurological effects.
- [[T3-NeonatalEpilepsy]] — the clinical consequence of failed anaplerotic compensation; ketogenic diet worsening is the most actionable clinical implication of this pathway node.

## Open questions

1. What is the mechanism by which ketogenic diet worsens DEE25 symptoms (Klotz-2016) — the single most clinically important unanswered question in this node? Hypotheses: (a) ketones reduce glutamine availability, impairing the primary anaplerotic route; (b) beta-oxidation of fatty acids from the ketogenic state generates mitochondrial acetyl-CoA that saturates TCA cycle without feeding the cytoplasmic citrate pool; (c) the ketogenic state alters CSF pH or electrolyte balance in a way that specifically worsens NaCT-deficient neurons.
2. Does glutamine supplementation in DEE25 neurons (iPSC-derived GABAergic neurons from patients) restore GABA synthesis capacity to levels approaching controls — specifically measurable by 13C-glutamine isotope tracing to track incorporation into GABA?
3. Can ACSS2 overexpression in SLC13A5-deficient developing neurons rescue nuclear acetyl-CoA levels and H3K27ac at synaptic gene loci — providing a gene therapy alternative that does not require NaCT restoration?
4. What is the metabolomic profile of DEE25 patients who improve on acetazolamide (4/9 in Klotz-2016) vs. those who do not — specifically, do acetazolamide responders have different TCA perturbation profiles at baseline, suggesting differential anaplerotic compensation?
