---
tags: [slc13a5-wiki, tier-2, pathway, transcription, PXR, AhR, TFAM, NRF2, regulation, liver, brain]
tier: 2
node_type: pathway
epistemic_status: established
last_updated: 2026-05-10
linked_nodes:
  - "[[T1-SLC13A5-GeneStructure]]"
  - "[[T1-ExpressionAtlas]]"
  - "[[T2-MitochondrialBioenergetics]]"
  - "[[T2-HepaticLipidMetabolism]]"
hypothesis_seeds:
  - "PXR agonism by phenobarbital (the most-used ASM in DEE25) simultaneously controls seizures AND upregulates hepatic SLC13A5 — an underappreciated pharmacodynamic interaction in patients already deficient for the same transporter"
  - "Brain-side TFAM/NRF2-like regulation of SLC13A5 means that mitochondrial biogenesis stimulators (resveratrol, NAD+ precursors) could upregulate SLC13A5 in neurons — a basis for testing them in DEE25 models"
open_questions:
  - "What transcription factor directly binds the SLC13A5 promoter in human cortical neurons — and does this factor's expression or activity decline with age, explaining the cerebrum expression trajectory observed by Ferreira-2026?"
  - "Is the SLC13A5 promoter accessible (open chromatin) in human iPSC-derived neurons from DEE25 patients — and does promoter methylation status differ between brain regions with different SLC13A5 expression levels?"
  - "Does resveratrol, NAD+ supplementation, or other mitochondrial biogenesis stimulators increase SLC13A5 expression in iPSC-derived neurons — and does this increase GABA synthesis capacity?"
---

# Transcriptional Regulation of SLC13A5

## Core claim

SLC13A5 transcription is controlled by distinct regulatory programs in liver and brain. In liver, PXR (pregnane X receptor) is the primary driver of phenobarbital-induced SLC13A5 expression, operating independently of the classical phenobarbital receptor CAR. AhR also induces hepatic SLC13A5. In brain, transcription factor target enrichment from WGCNA co-expression analysis implicates TFAM-associated genes and NFE2/NRF-like factors — the mitochondrial biogenesis and antioxidant response transcriptional program — though direct TF binding at the SLC13A5 promoter in brain has not been demonstrated. Sources: [[research/Li-2021-PXR]], [[research/Ferreira-2026]], [[mechanisms/SLC13A5-transcriptional-regulation]].

## Mechanism

**Liver regulatory program (✅ Established):**

PXR (NR1I2) is the primary driver of phenobarbital-induced SLC13A5 expression in human primary hepatocytes. Li-2021-PXR demonstrated this by receptor knockdown and selective agonist experiments:
- Phenobarbital induces SLC13A5 in human hepatocytes via PXR, not CAR (constitutive androstane receptor)
- This is mechanistically distinct from PB's induction of CYP2B6 and other drug-metabolizing enzymes (which are CAR-mediated)
- Other PXR agonists (rifampicin, St. John's wort, certain antiretrovirals) would also be predicted to induce hepatic SLC13A5

AhR (aryl hydrocarbon receptor) additionally induces SLC13A5 in liver (Li-Wang-2021). AhR is the receptor for polycyclic aromatic hydrocarbons and dioxins, but also has endogenous ligands. Both PXR and AhR are xenobiotic-sensing nuclear receptors; their action on SLC13A5 places hepatic citrate import under the xenobiotic response umbrella.

**Clinical implication — phenobarbital in DEE25 (💡 Speculative but mechanistically grounded):**
Phenobarbital is commonly used as an anti-seizure medication in DEE25 patients. It simultaneously: (1) inhibits GABA-A receptor desensitization and enhances GABAergic inhibition — therapeutic; (2) activates PXR → induces hepatic SLC13A5 expression — creates a paradoxical hepatic upregulation in patients who are constitutively SLC13A5-deficient. The significance of this is unclear: in biallelic LoF patients, the upregulated mRNA cannot produce functional protein regardless of transcriptional level. In heterozygous carriers, PB could upregulate the intact allele's expression in liver, potentially restoring hepatic NaCT to above-threshold levels. Whether this has any clinical consequence is not established.

**Brain regulatory program (🔶 Emerging — module-level enrichment only):**
Ferreira-2026 WGCNA TF target enrichment for the turquoise module (SLC13A5's module):
- NFE2/NRF-like motifs: Nrf2 (Nuclear factor erythroid 2-related factor 2) regulates antioxidant response element (ARE)-containing genes; relevant to mitochondrial protection
- TFAM-associated genes: TFAM (Transcription Factor A, Mitochondrial) is the master activator of mitochondrial genome transcription; nuclear TFAM binding sites (NRF1, NRF2 binding near TFAM-responsive elements) could co-regulate SLC13A5 alongside OXPHOS genes
- AP-1 family targets: AP-1 (FOS/JUN) is an activity-dependent transcription factor; could mediate activity-dependent SLC13A5 expression in neurons
- ELF1/BACH2: ELF1 is an ETS family TF; BACH2 is a BTB-domain repressor relevant to inflammatory and stress responses

This is module-level enrichment, not direct demonstration that any factor binds the SLC13A5 promoter. The implication: SLC13A5 expression in brain is co-regulated with mitochondrial biogenesis genes — if TFAM drives both, then TFAM activation (by exercise, NAD+ supplementation, resveratrol) could in principle upregulate neuronal SLC13A5.

## Evidence basis

- Source 1: [[research/Li-2021-PXR]] — direct demonstration of PXR (not CAR) as the PB-induced SLC13A5 driver in human hepatocytes.
- Source 2: [[research/Li-Wang-2021]] — comprehensive review of hepatic SLC13A5 regulation including AhR; hormonal and nutritional stimuli.
- Source 3: [[research/Ferreira-2026]] — WGCNA TF target enrichment; brain-side regulatory inferences.
- Source 4: [[mechanisms/SLC13A5-transcriptional-regulation]] — comprehensive mechanism page.

## Connections to other nodes

- [[T1-SLC13A5-GeneStructure]] — the regulatory elements (promoter, enhancers) that are the substrates for the TF binding described in this node.
- [[T1-ExpressionAtlas]] — the expression trajectories in different tissues reflect the regulatory programs described here: xenobiotic-receptor dominance in liver; TFAM/NRF2-like in brain.
- [[T2-MitochondrialBioenergetics]] — TFAM is the master mitochondrial transcription regulator; co-regulation of SLC13A5 with TFAM targets would place it in the same regulatory hub as OXPHOS genes.
- [[T2-HepaticLipidMetabolism]] — the hepatic xenobiotic receptor-driven SLC13A5 regulation means that certain drugs and environmental compounds could alter hepatic NaCT levels and thus hepatic lipid metabolism.

## Open questions

1. Which specific transcription factor(s) bind the SLC13A5 promoter in human cortical neurons — addressable by ChIP-seq from ENCODE or by direct ChIP in iPSC-derived neurons, targeting the candidate TFs (NRF2, TFAM, AP-1 components)?
2. Does CpG methylation of the SLC13A5 promoter or regulatory regions increase with aging in human brain, providing the epigenetic mechanism for the declining cerebrum expression trajectory observed by Ferreira-2026?
3. Are NRF2 activators (sulforaphane, dimethyl fumarate) able to induce SLC13A5 expression in human iPSC-derived cortical neurons — providing a pharmacological test of the TFAM/NRF-like regulatory hypothesis?
4. Does the phenobarbital-PXR-SLC13A5 induction pathway in liver affect plasma citrate levels in DEE25 patients on phenobarbital — measurable as a change in the diagnostic biomarker after drug initiation?
