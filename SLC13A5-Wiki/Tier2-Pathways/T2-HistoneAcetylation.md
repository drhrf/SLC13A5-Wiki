---
tags: [slc13a5-wiki, tier-2, pathway, histone-acetylation, epigenetics, H3K27ac, H3K9ac, neuroprotection, aging]
tier: 2
node_type: pathway
epistemic_status: emerging
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-AcetylCoAProduction]]"
  - "[[T2-MitochondrialBioenergetics]]"
  - "[[T3-IntellectualDisability]]"
  - "[[T4-AlzheimerDisease]]"
  - "[[T4-NeurodegenerationBroadly]]"
hypothesis_seeds:
  - "NaCT loss during the first postnatal year — the peak SLC13A5 expression window — reduces nuclear acetyl-CoA in developing neurons, permanently altering chromatin state at synaptic gene loci and explaining why developmental impairment does not recover even after seizures abate"
  - "H3K27ac ChIP-seq in iPSC neurons from DEE25 patients vs. isogenic controls would show reduced acetylation at enhancers of synaptic identity genes — the epigenetic scar hypothesis"
open_questions:
  - "Is H3K27ac or H3K9ac globally reduced in neurons from DEE25 patients, or are specific gene loci (synaptic, GABAergic, cholinergic identity genes) selectively affected?"
  - "Does ACLY inhibition in developing rodent neurons reproduce the chromatin phenotype of SLC13A5 loss — and does citrate supplementation rescue it?"
  - "What is the developmental time window during which altered histone acetylation from NaCT loss becomes irreversible — and does this window overlap with any therapeutic opportunity?"
---

# Histone Acetylation via Citrate-Derived Acetyl-CoA

## Core claim

Nuclear acetyl-CoA derived from citrate cleavage by ACLY (ATP-citrate lyase) is a substrate for histone acetyltransferases, which deposit H3K27ac and H3K9ac marks at enhancers and promoters of neuronal identity genes, synaptic function genes, and neuroprotective gene programs. Loss of citrate availability (as in SLC13A5 deficiency) is predicted to reduce nuclear acetyl-CoA and alter the chromatin landscape at these loci. This epigenetic mechanism is not yet directly demonstrated in SLC13A5-deficient neurons but is strongly supported by parallel evidence: ACSS2-derived acetyl-CoA sustains the same histone marks and protects neurons from tau-driven neurodegeneration. Sources: [[research/Pourshafie-2026]], [[mechanisms/acetyl-CoA-neurodegeneration]], [[research/Gul-Hinc-2026]].

## Mechanism

The metabolic-epigenetic axis in neurons:

1. **Substrate supply:** Cytoplasmic citrate (NaCT-imported or SLC25A1-derived) → ACLY → acetyl-CoA. In the cytoplasm, acetyl-CoA is used for ACh synthesis and fatty acid elongation. In the nucleus, acetyl-CoA is used by histone acetyltransferases (HATs: p300/CBP, PCAF, KAT families) to acetylate histone lysine residues.

2. **Key histone marks sensitive to acetyl-CoA availability:**
   - H3K27ac: enhancer activation mark; present at active neuronal enhancers including those controlling synaptic gene identity, GABAergic and cholinergic specification, and metabolic gene programs.
   - H3K9ac: gene body and promoter mark; associated with active transcription.
   - Global histone acetylation is sensitive to metabolic perturbations that alter the cytoplasmic/nuclear acetyl-CoA pool.

3. **ACSS2 as the established evidence anchor:** Pourshafie-2026 showed directly that ACSS2 overexpression in adult neurons maintains H3K9ac and H3K27ac at synaptic gene loci, that normal aging reduces nuclear ACSS2 activity (→ reduced histone acetylation → impaired gene regulation), and that tau pathology amplifies this deficit. ACSS2 uses acetate as substrate; ACLY uses citrate. Both feed the same nuclear acetyl-CoA pool.

4. **The developmental SLC13A5 connection (💡 Speculative):** The first postnatal year — the period of peak SLC13A5 cerebrum expression — is also the period of most active chromatin remodeling in developing neurons. Synaptic gene enhancers are programmed during this window. If NaCT loss reduces nuclear acetyl-CoA supply during this window, the chromatin state at synaptic loci is set incorrectly. The resulting epigenetic configuration is maintained by chromatin inheritance mechanisms and is not corrected even when seizures abate. This could explain why intellectual disability in DEE25 does not recover despite improved seizure control — the circuit-level impairment is encoded in chromatin, not just in ongoing neural activity.

5. **Aging intersection (🔶 Emerging):** The same mechanism applies across the lifespan in reverse: as SLC13A5 expression declines in aging brain, ACLY substrate falls, nuclear acetyl-CoA decreases, and histone acetylation at neuroprotective loci is reduced — analogous to the ACSS2 decline in aging described by Pourshafie-2026.

## Evidence basis

- Source 1: [[research/Pourshafie-2026]] — ACSS2 → H3K9ac/H3K27ac at synaptic gene loci; ACSS2 overexpression rescues cognitive decline from tau and aging; directly demonstrates the acetate-acetyl-CoA-histone axis in neurons. PMID 41512015.
- Source 2: [[mechanisms/acetyl-CoA-neurodegeneration]] — integrative synthesis proposing the citrate-ACLY-acetyl-CoA-histone chain as the epigenetic arm of the neurodegeneration hypothesis.
- Source 3: [[research/Gul-Hinc-2026]] — ACLY demonstrated as primary source of acetyl-CoA for ACh; same enzyme logically feeds nuclear acetyl-CoA, though the nuclear branch is not measured in this paper. PMID 41596431.
- Source 4: No vault source directly demonstrates histone acetylation changes in SLC13A5-deficient neurons. Claim derived from cross-domain inference (Pourshafie-2026 ACSS2 → ACLY parallel; developmental epigenetics literature). Requires primary literature verification.

## Connections to other nodes

- [[T2-AcetylCoAProduction]] — upstream; this node is the direct downstream of ACLY-generated acetyl-CoA; the supply is established in the parent node.
- [[T2-MitochondrialBioenergetics]] — the OXPHOS module that co-expresses with SLC13A5 (Ferreira-2026) includes mitochondrial biogenesis regulators (TFAM) whose targets overlap with the TF enrichment seen in the SLC13A5 module; both bioenergetics and epigenetics are under similar transcriptional control.
- [[T3-IntellectualDisability]] — the epigenetic programming hypothesis offers a mechanistic explanation for the irreversibility of intellectual disability in DEE25, which is otherwise unexplained by the seizure-damage model.
- [[T4-AlzheimerDisease]] — reduced nuclear acetyl-CoA in aging neurons → impaired histone acetylation → dysregulated synaptic gene expression → cognitive decline; this is the epigenetic arm of the AD-connection hypothesis.
- [[T4-NeurodegenerationBroadly]] — the ACSS2-aging paper (Pourshafie-2026) establishes the principle across neurodegeneration; NaCT-ACLY is the additional upstream node.

## Open questions

1. Does SLC13A5 loss in iPSC-derived cortical neurons from DEE25 patients produce measurable reductions in H3K27ac signal at synaptic gene enhancers — detectable by CUT&RUN or ChIP-seq in relevant patient iPSC lines available through [[research/Beltran-2024]]?
2. Is the irreversibility of developmental intellectual disability in DEE25 epigenetically encoded — specifically, does restoring NaCT activity after the critical window (e.g., adult AAV gene therapy in the mouse model, [[research/Bailey-2026]]) fail to rescue any epigenetic marks even when seizures are controlled?
3. Does ACSS2 expression increase in SLC13A5-deficient developing neurons as a compensatory response to reduced ACLY substrate — and if so, does this compensation fully or partially rescue synaptic gene histone acetylation?
4. Is there a direct link between citrate availability and HAT enzyme activity — do any known HATs have citrate as an allosteric regulator, independent of the acetyl-CoA supply effect?
