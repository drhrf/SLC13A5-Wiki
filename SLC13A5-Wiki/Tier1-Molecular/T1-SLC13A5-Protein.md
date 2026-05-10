---
tags: [slc13a5-wiki, tier-1, molecular, protein, structure, NaCT, cryo-EM]
tier: 1
node_type: molecular
epistemic_status: established
last_updated: 2026-05-10
linked_nodes:
  - "[[T1-SLC13A5-GeneStructure]]"
  - "[[T1-VariantCatalog]]"
  - "[[T2-CitrateTCAIntegration]]"
  - "[[T2-NMDAModulation]]"
  - "[[T1-InteractingProteins]]"
hypothesis_seeds:
  - "The elevator mechanism of NaCT transport creates a gating intermediate that could be targeted by allosteric modulators distinct from substrate-competitive inhibitors"
  - "Na1 and Na2 site asymmetry could enable sodium-concentration-sensitive modulation of citrate transport relevant to seizure physiology"
open_questions:
  - "What is the outward-facing conformation of NaCT? The published cryo-EM structures are both inward-facing — the alternating-access mechanism is inferred but not directly visualized."
  - "Does the NaCT homodimer cooperate during transport (coupled protomer movements) or do protomers function independently?"
  - "At physiological extracellular citrate concentrations (~100-200 µM in CSF), what fraction of NaCT sites are occupied — and does this change in SLC13A5 deficiency due to citrate accumulation?"
---

# SLC13A5 Protein (NaCT)

## Core claim

NaCT is an 11-transmembrane domain sodium-coupled citrate transporter encoded by SLC13A5. Its atomic structure was resolved by cryo-EM at 3.04 Å (citrate-bound) and 3.12 Å (inhibitor-bound), revealing an elevator transport mechanism with two Na⁺ binding sites and a citrate pocket that is the target of all known competitive inhibitors. The human transporter has markedly higher transport capacity than the mouse ortholog — the central species-difference caveat for all animal model data. Sources: [[research/Sauer-2021]], [[genes/SLC13A5]], [[mechanisms/citrate-transport]].

## Mechanism

NaCT operates as a homodimer (125 kDa total). Each protomer contains two functional domains: a **scaffold domain** (TM1–4 + TM7–9) that forms the rigid membrane-anchored framework, and a **transport domain** (TM5, TM6, TM10, TM11 + hairpins HP1/HP2) that moves as a rigid body relative to the scaffold — the elevator mechanism — to alternately expose the substrate-binding site to extracellular and intracellular compartments.

Transport is electrogenic: three Na⁺ ions are co-transported with one citrate³⁻, making the overall process dependent on the electrochemical Na⁺ gradient and membrane potential. Na⁺ binds at two sites (Na1 and Na2) coordinated by SNT (Ser-Asn-Thr) signature motifs conserved across the SLC13 family. Citrate³⁻ binds in the HP1/HP2 clamshell region, coordinated by multiple backbone and side-chain contacts.

Substrate selectivity: citrate >> succinate > α-ketoglutarate. The four scaffold domain residues Leu56, Ala57, Gly409, and Ile410 create a binding pocket geometry that favors the tricarboxy citrate over dicarboxy substrates, explaining selectivity over NaDC1 and NaDC3. The Pfizer inhibitor PF-06649298 (compound 2) occupies the citrate site competitively — it is itself a substrate analog, not an allosteric inhibitor.

Transport kinetics in mouse mINDY (HEK293 system): citrate Km = 49 µM, Vmax = 3760 pmol/(mg·min); succinate Km = 105 µM, Vmax = 443 pmol/(mg·min). Human NaCT has markedly higher Vmax than mouse — the mechanistic basis of the species difference that makes human SLC13A5 loss catastrophic while mouse Slc13a5 loss is mild. Sources: [[research/Birkenfeld-2011]], [[research/Sauer-2021]], [[research/Kopel-2021]].

## Evidence basis

- Source 1: [[research/Sauer-2021]] — cryo-EM structures (PDB: 7JSK, 7JSJ; EMDB: EMD-22457, EMD-22456); defines homodimer architecture, Na+ sites, citrate pocket, elevator mechanism, inhibitor mechanism.
- Source 2: [[research/Birkenfeld-2011]] — HEK293 kinetic measurements for mINDY; Km/Vmax for citrate and succinate.
- Source 3: [[genes/SLC13A5]] — integrative summary of protein structure, species capacity difference, and inhibitor landscape.
- Source 4: [[research/Wang-2025]] — deep mutational scanning (DMS) of 9,707/10,773 possible single amino acid substitutions; validates all known patient variants as transport-deficient; establishes blood citrate as NaCT activity proxy (r = −0.63 in UK Biobank).
- Source 5: [[mechanisms/citrate-transport]] — mechanistic overview including dominant-negative behavior of pathogenic variants.

## Connections to other nodes

- [[T1-SLC13A5-GeneStructure]] — the gene encodes this protein; domain boundaries correspond to exonic structure.
- [[T1-VariantCatalog]] — all pathogenic variants map to specific structural positions; Class I/II classification is directly interpretable from protein structure.
- [[T2-CitrateTCAIntegration]] — NaCT is the entry point for extracellular citrate into cytoplasmic metabolic pools; the protein's transport kinetics set the rate of citrate entry.
- [[T2-NMDAModulation]] — citrate exported to CSF (when NaCT is absent and cannot clear it) modulates zinc and NMDA receptor function; the protein's transport direction is the central variable.
- [[T1-InteractingProteins]] — dominant-negative coexpression of WT and mutant NaCT subunits is a protein-level interaction with direct therapeutic implications.

## Open questions

1. What does the outward-facing (extracellular-open) conformation of NaCT look like? All published cryo-EM data captures the inward-facing state; the alternating-access mechanism requires characterizing the full transport cycle.
2. Does the homodimer show cooperative kinetics — do the two protomers communicate during citrate translocation, or is each independent? Cooperativity would create a Hill coefficient > 1 in transport-rate-vs-concentration curves.
3. At the physiological CSF citrate concentration observed in humans (~100–200 µM, rising with age per [[research/Lin-2021]]), what fraction of NaCT sites are occupied? This determines how far the transporter operates below saturation in vivo and whether the aging rise in CSF citrate reflects reduced NaCT activity, reduced NaCT expression, or both.
4. What is the structural basis of the dominant-negative suppression of WT NaCT by co-expressed pathogenic mutants — does the mutant subunit trap the WT subunit in a non-productive conformation, or disrupt plasma membrane targeting of the dimer?
