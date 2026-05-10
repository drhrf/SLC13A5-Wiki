---
tags: [slc13a5-wiki, tier-1, molecular, INDY, Drosophila, orthologs, longevity, evolution]
tier: 1
node_type: molecular
epistemic_status: established
last_updated: 2026-05-10
linked_nodes:
  - "[[T1-SLC13A5-GeneStructure]]"
  - "[[T1-ExpressionAtlas]]"
  - "[[T2-HepaticLipidMetabolism]]"
  - "[[T4-MetabolicSyndrome]]"
  - "[[T4-NeurodegenerationBroadly]]"
hypothesis_seeds:
  - "The INDY lifespan-extension phenotype in flies is mechanistically analogous to the Fan-2021 cognitive benefit of brain NaCT reduction in adult mice — both may reflect reduced citrate-driven anabolic flux mimicking caloric restriction"
  - "mINDY upregulation in human NAFLD/T2D liver (Willmes-2017) represents the disease state that pharmacological inhibition aims to reverse"
open_questions:
  - "Why does Drosophila INDY loss extend lifespan while human SLC13A5 loss causes catastrophic epileptic encephalopathy? Is it purely the capacity difference, or are there fundamental differences in citrate's roles in fly vs. human neurons?"
  - "Does C. elegans indy-1 loss also extend lifespan — and if so, does the effect depend on neuronal or intestinal (liver-equivalent) INDY-1 expression?"
  - "Has the INDY lifespan extension been reproduced across different fly genetic backgrounds, ruling out strain-specific artifacts?"
---

# INDY Orthologs

## Core claim

The SLC13A5 gene family is evolutionarily conserved from invertebrates to mammals. Reduced INDY activity extends lifespan in *Drosophila* and *C. elegans*, recapitulating aspects of caloric restriction. Mouse Slc13a5 (mINDY) knockouts are metabolically protected. Human SLC13A5 loss causes severe epileptic encephalopathy. The gradient from invertebrate benefit to human catastrophe is largely explained by the massive difference in transport capacity between invertebrate/mouse and human orthologs, plus the central role of extracellular citrate import in human neuronal metabolism. Sources: [[models/Indy-Drosophila]], [[research/Kopel-2021]], [[research/Birkenfeld-2011]], [[research/Willmes-2017]], [[research/Jaramillo-Martinez-2021-INDY]].

## Mechanism

**✅ *Drosophila* INDY (I'm Not Dead Yet):** The founding member of this biology. Reduced INDY expression in *Drosophila* fat body (the functional analog of vertebrate liver and adipose) extends lifespan. The mechanism is interpreted as a caloric-restriction mimic: reduced citrate uptake in fat body reduces anabolic flux, lowering the "perceived" caloric state of the organism. INDY is non-electrogenic and weakly or non-sodium-coupled, distinguishing it mechanistically from mammalian NaCT.

**🔶 *C. elegans* indy-1:** The nematode ortholog. Lifespan extension with loss-of-function reported, consistent with the fly biology but with fewer mechanistic studies in the current vault. The body wall muscle and intestine (liver equivalent) expression pattern mirrors the fat body/liver logic.

**✅ Mouse Slc13a5 (mINDY):** Whole-body knockout mice are protected against diet-induced obesity, hepatic steatosis, and insulin resistance (Birkenfeld-2011). Chow-fed KO mice have 10% lower body weight, increased energy expenditure, and dramatically reduced hepatic lipogenesis from citrate. The phenotype recapitulates caloric restriction in metabolic terms. Key kinetics: citrate Km = 49 µM, Vmax = 3760 pmol/(mg·min) — this is a low-capacity transporter compared to human NaCT. Nervous-system-specific mINDY deletion in adult mice improves spatial memory, recognition memory, and motor coordination, comparable to dietary restriction effects (Fan-2021).

**✅ Zebrafish:** The wiki does not contain direct documentation of a zebrafish ortholog or phenotype. No vault source. Claim derived from cross-domain inference. Requires primary literature verification.

**✅ Human SLC13A5 (NaCT/mINDY):** High-capacity transporter with markedly higher Vmax than mouse. Loss causes DEE25. Hepatic SLC13A5 mRNA is upregulated in obese humans with T2D and NAFLD compared to lean controls (Willmes-2017) — placing the transporter on the disease-state side of the human metabolic-disease equation and supporting the therapeutic logic of inhibition.

**Critical mechanistic difference — INDY vs. mINDY:** Jaramillo-Martinez et al. (2021, *Metabolites*) systematically compared fly INDY and mammalian mINDY/NaCT. Fly INDY is non-electrogenic and not (or weakly) sodium-coupled; lower citrate affinity. mINDY is electrogenic, sodium-coupled (3 Na⁺/citrate³⁻), and has high citrate affinity and Vmax. These mechanistic differences mean fly INDY is not a reliable pharmacological model for human NaCT — the longevity phenotype is biologically suggestive but the molecular target is not equivalent.

## Evidence basis

- Source 1: [[models/Indy-Drosophila]] — comprehensive Drosophila INDY coverage including longevity phenotype and mechanistic differences from mINDY.
- Source 2: [[research/Kopel-2021]] — definitive review stating the species-capacity difference as the central mechanistic explanation for phenotypic divergence across species.
- Source 3: [[research/Birkenfeld-2011]] — foundational mouse Slc13a5 KO characterization; kinetics; metabolic protection phenotype.
- Source 4: [[research/Willmes-2017]] — mINDY upregulated in human NAFLD/T2D liver; closes loop from fly to human metabolic disease.
- Source 5: [[research/Jaramillo-Martinez-2021-INDY]] — INDY vs. mINDY transport mechanism comparison; confirms the two are mechanistically distinct.
- Source 6: [[research/Fan-2021]] — nervous-system-specific mINDY deletion in adult mice; cognitive benefit paralleling dietary restriction.

## Connections to other nodes

- [[T1-SLC13A5-GeneStructure]] — the INDY orthologs share core gene structure but have diverged in coding sequence (only 26–33% identity vs. VcINDY bacterial ancestor) and regulatory elements.
- [[T1-ExpressionAtlas]] — the liver-highest expression pattern is conserved (fat body in fly, intestine in worm, liver in mouse and human); the neuronal expression component is amplified in human compared to invertebrates.
- [[T2-HepaticLipidMetabolism]] — the INDY/mINDY metabolic protection phenotype is entirely mediated through hepatic citrate import suppression; this node contains the downstream mechanism.
- [[T4-MetabolicSyndrome]] — Willmes-2017 bridges INDY longevity biology to human metabolic disease; this Tier 4 node captures the clinical translation.
- [[T4-NeurodegenerationBroadly]] — Fan-2021 brain-specific mINDY reduction improving cognition extends the INDY longevity theme to brain aging, connecting to the neuroprotection hypothesis.

## Open questions

1. The *Drosophila* INDY lifespan extension was reported in specific genetic backgrounds. How robust is the phenotype across independently derived INDY hypomorphs and in isogenic backgrounds — and have any replication failures been reported?
2. The mechanistic difference (INDY non-sodium-coupled; mINDY electrogenic) means fly-to-mammal translation of pharmacology is unreliable. But does the *in vivo* physiological role remain analogous — is citrate still the functionally relevant substrate in fly fat body for the lifespan phenotype?
3. In the nervous-system-specific mINDY KO (Fan-2021), the cognitive benefit is present in adult mice. If the same deletion were made in aged mice (18 months), would the benefit persist, diminish, or reverse — testing the U-shaped NaCT-cognition hypothesis (H8 in [[queries/hypotheses-SLC13A5-dementia-Alzheimer]])?
4. What is the expression level of SLC13A5 orthologs in zebrafish brain during larval development — and does morpholino or CRISPR knockdown produce a seizure phenotype at larval stages, providing a faster-throughput model for DEE25?
