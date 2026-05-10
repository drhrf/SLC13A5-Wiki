---
tags: [slc13a5-wiki, tier-1, molecular, protein-interactions, ACLY, ACSS2, ZIP1, SLC25A1, dominant-negative]
tier: 1
node_type: molecular
epistemic_status: emerging
last_updated: 2026-05-10
linked_nodes:
  - "[[T1-SLC13A5-Protein]]"
  - "[[T2-AcetylCoAProduction]]"
  - "[[T2-HepaticLipidMetabolism]]"
  - "[[T3-ToothEnamelHypoplasia]]"
hypothesis_seeds:
  - "ACLY and NaCT form a functional metabolic unit in neurons — physical proximity at the cytoplasmic face of the plasma membrane could enable substrate channeling from citrate import to acetyl-CoA production"
  - "ZIP1 upregulation in SLC13A5-deficient osteoblasts is an adaptive response that could be pharmacologically targeted to partially normalize bone citrate partitioning without restoring NaCT"
open_questions:
  - "Does NaCT physically interact with ACLY at the cytoplasmic membrane face in neurons — and if so, does this interaction channel citrate preferentially to ACLY vs. other cytoplasmic citrate-utilizing enzymes?"
  - "What mediates the dominant-negative suppression of WT NaCT by pathogenic mutant subunits — is it dimerization-dependent (dominant-negative protomer trapping the WT in a non-transport state) or expression-level competition?"
  - "Are there regulatory proteins that modify NaCT transport activity post-translationally — phosphorylation, ubiquitination, or protein-protein interactions that tune the transporter in response to metabolic state?"
---

# Interacting Proteins

## Core claim

NaCT's functional interactions extend beyond its role as a standalone transporter. Key molecular partners include: ATP-citrate lyase (ACLY), which converts NaCT-imported citrate to acetyl-CoA; ACSS2, which provides a parallel acetate-derived acetyl-CoA route in neurons; SLC25A1, the mitochondrial citrate carrier that works complementarily with NaCT; ZIP1, the zinc importer whose upregulation compensates for SLC13A5 loss in osteoblasts via cataplerosis; and mutant NaCT subunits themselves, which suppress WT NaCT through dominant-negative dimerization. Sources: [[mechanisms/acetyl-CoA-neurodegeneration]], [[research/Dirckx-2022]], [[mechanisms/citrate-transport]], [[research/Gul-Hinc-2026]], [[research/Pourshafie-2026]].

## Mechanism

**✅ ACLY (ATP-citrate lyase):** The immediate downstream enzyme that converts cytoplasmic citrate to acetyl-CoA + oxaloacetate. In cholinergic neurons, ACLY is the primary source of acetyl-CoA for acetylcholine synthesis, demonstrated by isotope tracing and validated by strong regional correlation between ACLY activity and ChAT activity across brain regions (Gul-Hinc-2026). ACLY is present at presynaptic terminals, suggesting local acetyl-CoA generation near the site of ACh synthesis. NaCT and ACLY thus form a functional metabolic unit: NaCT supplies the substrate (citrate) that ACLY converts to the product (acetyl-CoA) required for neurotransmission.

**🔶 ACSS2 (acetyl-CoA synthetase 2):** A parallel route to nuclear acetyl-CoA from acetate, independent of citrate. ACSS2 overexpression protects neurons from tau-driven cognitive decline by sustaining histone acetylation at synaptic gene loci (Pourshafie-2026). ACLY and ACSS2 are alternative suppliers of the same nuclear acetyl-CoA pool — reduced ACLY flux from NaCT loss could in principle be partially compensated by ACSS2 upregulation. Whether compensatory ACSS2 upregulation occurs in SLC13A5-deficient neurons is not documented in the vault.

**✅ SLC25A1 (mitochondrial citrate carrier):** The inner-mitochondrial-membrane transporter that exports mitochondria-derived citrate to the cytoplasm. SLC25A1 provides an endogenous source of cytoplasmic citrate that does not depend on NaCT-mediated extracellular import. In osteoblasts, SLC25A1 is upregulated in Slc13a5 KO mice as part of the compensatory ZIP1/cataplerosis pathway (Dirckx-2022). In neurons, SLC25A1 is the presumed source of cytoplasmic citrate under conditions where NaCT is absent — but whether this source is quantitatively sufficient to maintain ACLY flux in human neurons (given the high-capacity NaCT) is the central open question.

**✅ ZIP1 (SLC39A1, zinc importer):** Identified in osteoblasts as the mediator of the compensatory cataplerosis response to SLC13A5 loss. When NaCT cannot import extracellular citrate, ZIP1-mediated zinc uptake inhibits mitochondrial aconitase → citrate accumulates in mitochondria → exported via SLC25A1 → secreted into the mineral matrix. ZIP1/SLC13A5 double-KO rescues bone phenotype, directly validating the pathway. ZIP1 is also expressed in neurons, where synaptic zinc release is a physiologically important signal — the interaction between zinc, citrate chelation, and NaCT function in neurons extends from the osteoblast finding (see [[T2-ZincCitrateInteraction]]).

**💡 NaCT homodimer dominant-negative:** Co-expression of WT and pathogenic Class I mutant NaCT subunits (e.g., p.Cys50Arg) suppresses WT NaCT expression and transport activity beyond what would be expected from haploinsufficiency (Klotz-2016). The mechanism is not fully characterized — it may involve heterodimer formation trapping WT subunits in a non-productive conformation, or competition for dimer-stabilizing chaperones. This interaction constrains gene therapy strategies: adding WT SLC13A5 into cells expressing Class I mutants may not achieve full transport rescue.

**🔶 NKCC1/KCC2 (SLC12A2/SLC12A5):** Indirect functional interaction. NKCC1 and KCC2 control intraneuronal Cl⁻ concentration and hence the polarity of GABA signaling (excitatory at high [Cl⁻]ᵢ, inhibitory at low [Cl⁻]ᵢ). The GABA polarity switch in development depends on KCC2 replacing NKCC1. NaCT's role in supplying GABA synthesis precursors (via TCA anaplerosis) intersects with the KCC2/NKCC1 system during the critical window when GABAergic inhibition is being established — the H1 developmental hypothesis (see [[queries/hypotheses-SLC13A5-developmental-disorders]]).

## Evidence basis

- Source 1: [[research/Gul-Hinc-2026]] — ACLY as primary acetyl-CoA source for ACh in cholinergic neurons; ACLY at presynaptic terminals; regional ACLY-ChAT correlation.
- Source 2: [[research/Pourshafie-2026]] — ACSS2 → nuclear acetyl-CoA → histone acetylation → neuroprotection; parallel route to ACLY.
- Source 3: [[research/Dirckx-2022]] — ZIP1 and SLC25A1 as compensatory osteoblast partners; ZIP1 KO rescue experiment.
- Source 4: [[research/Klotz-2016]] — dominant-negative coexpression of WT and mutant NaCT subunits; first description of this interaction.
- Source 5: [[mechanisms/acetyl-CoA-neurodegeneration]] — synthesis of ACLY/ACSS2 interactions in the neurodegeneration context.

## Connections to other nodes

- [[T1-SLC13A5-Protein]] — all these interactions are at the protein level; the dominant-negative interaction requires the homodimer architecture established in Sauer-2021.
- [[T2-AcetylCoAProduction]] — ACLY and ACSS2 are the primary players in this Tier 2 node, which extends the NaCT → citrate → acetyl-CoA pathway mechanistically.
- [[T2-HepaticLipidMetabolism]] — ACLY is equally central in liver, where citrate → acetyl-CoA → fatty acid synthesis is the main anabolic flux; NaCT-ACLY coupling is functionally analogous in hepatocytes.
- [[T3-ToothEnamelHypoplasia]] — ZIP1 interaction in osteoblasts is the mechanistic explanation for the paradoxically elevated mineral citrate in KO teeth.

## Open questions

1. Does NaCT physically interact with ACLY in neurons — co-immunoprecipitation or proximity ligation assay data do not exist in the current vault. Physical proximity at the cytoplasmic face of the plasma membrane would suggest substrate channeling (citrate passing from NaCT directly to ACLY without diffusing into the bulk cytoplasm).
2. Is ACSS2 upregulated in SLC13A5-deficient neurons as a compensatory response to reduced ACLY substrate availability — and if so, does this compensation prevent epigenetic programming defects in developing brain?
3. What is the kinetic competition between ACLY and TCA-cycle re-entry for NaCT-derived cytoplasmic citrate in neurons — does the neurotransmitter biosynthesis function (ACh) compete with energy metabolism for the same substrate?
4. Does the dominant-negative NaCT interaction depend on the dimer interface residues identified in Sauer-2021 (Arg76–Asp85', Trp408–Trp408') — and if so, could a monomeric NaCT construct bypass this limitation for gene therapy?
