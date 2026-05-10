---
tags: [slc13a5-wiki, tier-1, molecular, variants, pathogenic, DMS, genotype-phenotype]
tier: 1
node_type: molecular
epistemic_status: established
last_updated: 2026-05-10
linked_nodes:
  - "[[T1-SLC13A5-Protein]]"
  - "[[T3-NeonatalEpilepsy]]"
  - "[[T3-IntellectualDisability]]"
  - "[[T3-ToothEnamelHypoplasia]]"
hypothesis_seeds:
  - "Class II variants (ER-retained) may respond to pharmacological chaperones — low-temperature rescue proof-of-concept exists for p.Leu488Pro"
  - "Dominant-negative suppression by Class I variants constrains AAV gene therapy dosing and design"
  - "Common partially-damaging SLC13A5 alleles (DMS score intermediate) may modify cognitive aging risk in the general population"
open_questions:
  - "Why is there no genotype-phenotype correlation despite >50 distinct LoF variants? Are all variants truly equivalent in residual transport function?"
  - "What fraction of DEE25 patients have CNV (whole-gene deletion) as the cause, and how many are missed by standard sequencing panels?"
  - "Do the 12 VUSs reclassified as neutral by Wang-2025 DMS include any that were used to make diagnostic or therapeutic decisions in patients?"
---

# Variant Catalog

## Core claim

More than 50 loss-of-function variants in SLC13A5 cause DEE25. These fall into two mechanistic classes: Class I (protein reaches the plasma membrane but cannot transport citrate) and Class II (protein is ER-retained and degraded). All tested variants result in severe loss of transport function with no genotype-phenotype correlation established across the 145 patients in the TESS database. Deep mutational scanning covers 90% of all possible single amino acid substitutions and validates blood citrate as a population-level proxy for NaCT function. Sources: [[research/Jaramillo-Martinez-2024]], [[research/Wang-2025]], [[research/Klotz-2016]], [[research/Matricardi-2020]], [[conditions/SLC13A5-deficiency]].

## Mechanism

Pathogenic variants in SLC13A5 cause DEE25 through one of two mechanisms identified by Jaramillo-Martinez et al. 2024:

**Class I — membrane-present, transport-dead:** The variant protein is correctly folded and traffics to the plasma membrane but fails to transport citrate. Examples: p.Cys50Arg, p.Thr142Met, p.Thr227Met. These affect residues that form the sodium-binding sites or the citrate coordination pocket, so the elevator mechanism fails despite normal membrane localization. Therapeutic implication: restoring transport function (e.g., pharmacological stabilization of the active conformation) is needed; gene replacement is complicated by dominant-negative risk because co-expressed mutant subunits suppress WT NaCT activity.

**Class II — ER-retained, proteasomally degraded:** The variant protein misfolds in the ER and is targeted for ERAD (ER-associated degradation). Examples: p.Gly219Arg, p.Ser427Leu, p.Leu488Pro. mRNA levels are normal — the defect is post-translational. Low-temperature (27°C) partially rescues folding and transport activity (Leu488Pro > Ser427Leu > Gly219Arg), suggesting thermodynamic rather than absolute structural incompatibility. Therapeutic implication: pharmacological chaperones that stabilize the folding intermediate could rescue this class; gene replacement bypasses the defect entirely.

**Dominant-negative effect (Class I relevant):** Co-expression of WT and mutant NaCT subunits suppresses WT protein expression and transport activity more than would be expected from simple haploinsufficiency. This was first reported by Klotz-2016 and mechanistically constrains both gene therapy (adding WT copies into cells expressing mutant subunits may be partially blocked) and protein replacement strategies.

**CNV class:** One family reported by Duan-2021 had whole-gene deletion by Alu/Alu-mediated rearrangement — a structural variant missed by standard SNV/indel exome panels. Chromosomal microarray or CNV-aware analysis is required for complete variant detection.

**Deep mutational scanning (DMS):** Wang-2025 (*Sci Adv* 2025) performed comprehensive DMS of SLC13A5 covering 9,707/10,773 possible single amino acid substitutions (90% coverage). Key outputs: 28.4% of variants classified highly deleterious (FDR 4.9%); ~60% classified neutral (FDR 23%); all known patient variants confirmed transport-deficient; 12 VUSs reclassified as neutral. Blood citrate in UK Biobank participants negatively correlates with DMS functional score (r = −0.63 for alleles with minor allele count >25) — population-level validation that blood citrate reports NaCT function.

## Evidence basis

- Source 1: [[research/Jaramillo-Martinez-2024]] — Class I/II mechanistic classification; 145 TESS patients; 35 confirmed missense variants.
- Source 2: [[research/Wang-2025]] — DMS covering 90% of variants; UK Biobank blood-citrate validation; VUS reclassification.
- Source 3: [[research/Klotz-2016]] — early variant characterization cohort; dominant-negative effect first described.
- Source 4: [[research/Matricardi-2020]] — 14-patient natural history cohort with variant distribution (8 compound heterozygotes, 6 homozygotes).
- Source 5: [[variants/p.Cys50Arg]], [[variants/p.Thr142Met]], [[variants/p.Thr227Met]] — Class I variants.
- Source 6: [[variants/p.Gly219Arg]], [[variants/p.Ser427Leu]], [[variants/p.Leu488Pro]] — Class II variants (most common is p.Gly219Arg).
- Source 7: [[research/Duan-2021]] — CNV variant (whole-gene deletion) identifying structural variant class.
- Source 8: [[research/He-2025]] — p.Glu569ext174 (nonstop extension variant, unclassified by Class I/II system).

## Connections to other nodes

- [[T1-SLC13A5-Protein]] — all pathogenic variants map to structural positions in the cryo-EM model; Class I/II distinction maps to protein folding vs. transport mechanism failure.
- [[T3-NeonatalEpilepsy]] — all Class I and II variants produce the same neonatal epilepsy onset, explaining the lack of genotype-phenotype correlation.
- [[T3-IntellectualDisability]] — intellectual disability is universal despite different variant mechanisms, again reflecting convergence on near-complete loss of transport.
- [[T3-ToothEnamelHypoplasia]] — dental phenotype is consistent across all variants regardless of class, because ameloblast function requires NaCT transport regardless of the molecular mechanism of its loss.

## Open questions

1. Why does the dominant-negative effect (Class I variants suppressing WT NaCT in co-expression) not produce more severe disease in compound heterozygotes carrying one Class I and one Class II allele, given that the Class I protein is present at the membrane and can suppress the WT? Does the Class II allele fail to produce protein that reaches the dimer, reducing the effective dominant-negative burden?
2. At what allele frequency does partially-damaging SLC13A5 variants (DMS score intermediate, e.g., 0.3–0.7 of WT) contribute to sub-clinical citrate transport deficiency in the general population — and does this frequency vary across ancestry groups in ways that predict cognitive aging trajectories?
3. Are there modifier variants in genes encoding ACLY, ACSS2, or other citrate-utilizing enzymes that explain phenotypic variability among patients with identical SLC13A5 genotypes?
4. Has the nonstop variant p.Glu569ext174 (He-2025) been biochemically characterized for Class I/II assignment, and what does its transport activity tell us about the C-terminal region of NaCT?
