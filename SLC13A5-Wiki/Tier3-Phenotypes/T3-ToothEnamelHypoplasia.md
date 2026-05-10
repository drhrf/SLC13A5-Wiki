---
tags: [slc13a5-wiki, tier-3, phenotype, tooth, enamel, amelogenesis-imperfecta, biomarker, bone, citrate-mineralization]
tier: 3
node_type: phenotype
epistemic_status: established
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-CitrateTCAIntegration]]"
  - "[[T2-ZincCitrateInteraction]]"
  - "[[T1-ExpressionAtlas]]"
hypothesis_seeds:
  - "DEE25 tooth enamel micro-CT density could serve as a cheap, non-invasive biomarker for monitoring NaCT activity level and response to gene therapy — enamel mineral density reflects the lifetime integrated NaCT function during tooth development"
  - "Bone density is likely reduced in DEE25 patients for the same mechanism as enamel — systematic bone densitometry (DXA) in DEE25 should be a standard clinical assessment"
open_questions:
  - "Is bone mineral density systematically reduced in DEE25 patients — and does this correlate with fracture risk or growth trajectory in longitudinal follow-up?"
  - "Does partial NaCT restoration (e.g., gene therapy) improve enamel or bone density in teeth or bones that form after the therapeutic intervention — making these a biological readout of treatment effect?"
  - "Is the tooth phenotype in DEE25 distinguishable from Kohlschütter-Tönz syndrome due to ROGDI mutations by micro-CT density analysis — potentially providing a diagnostic discriminator?"
---

# Tooth Enamel Hypoplasia and Bone Involvement

## Core claim

Tooth hypoplasia or hypodontia (often classified as amelogenesis imperfecta) is the distinctive recognizable feature of DEE25, present alongside neonatal seizures and developmental delay. Dirckx-2022 provides the complete mechanistic explanation: SLC13A5 is expressed in ameloblasts (enamel-secreting) and odontoblasts (dentin-secreting); NaCT loss in these cells dysregulates citrate partitioning through a ZIP1-driven cataplerosis pathway, producing paradoxically elevated mineral citrate and defective crystal growth — absence of enamel in KO mice and significantly reduced enamel and dentin thickness and density in DEE25 primary teeth. Bone mechanical integrity is also compromised. Sources: [[research/Dirckx-2022]], [[research/Hardies-2015]], [[research/Matricardi-2020]], [[research/Irizarry-2017]].

## Mechanism

**Why citrate matters in mineralized tissues (✅ Established — Dirckx-2022):**
>85% of total body citrate is stored in bone mineral (carbonated hydroxyapatite). Citrate is the most abundant organic molecule in bone, bound to apatite crystal surfaces where it restricts crystal thickening and regulates crystal growth dimensions. Both too little and too much citrate is detrimental — the physiological role of citrate in bone is to control crystal size, not simply to be incorporated.

**NaCT in mineralizing cells (✅ Established):**
- SLC13A5 is highly expressed in osteoblasts, ameloblasts, and odontoblasts
- Expression rises during osteoblast differentiation and peaks in mineralizing osteoblasts
- Ameloblast expression confirmed by immunohistochemistry; ablation in osteocalcin-Cre conditional KO spares enamel (ameloblasts lack osteocalcin-Cre recombination) but still affects dentin

**The paradox — too much mineral citrate in KO (✅ Established):**
Counterintuitively, SLC13A5 KO osteoblasts have 4-fold more mineral citrate, not less. The mechanism:
1. NaCT absent → no extracellular citrate import → reduced cytoplasmic citrate
2. Reduced cytoplasmic citrate → derepressed PFK → increased glycolysis → more acetyl-CoA → TCA entry → increased mitochondrial citrate synthesis
3. ZIP1-mediated zinc uptake → inhibits mitochondrial aconitase → citrate cannot proceed to isocitrate → citrate accumulates in mitochondria
4. SLC25A1 exports excess mitochondrial citrate → secretion into the mineral matrix
5. Excess mineral citrate → aberrant hydroxyapatite crystal formation → mechanically weak bone; enamel deficiency

The ZIP1 cataplerosis pathway is directly validated: ZIP1 KO alone has no bone phenotype; ZIP1 in Slc13a5 KO background rescues bone cortical thickness and mechanical strength.

**Human DEE25 tooth phenotype (✅ Established — Dirckx-2022):**
Micro-CT of primary teeth from 5 DEE25 children vs. 10 age/sex-matched controls:
- Reduced enamel thickness (significant)
- Reduced enamel density (significant)
- Reduced dentin thickness (significant)
- Reduced dentin density (significant)

**Clinical discriminator value:**
Tooth hypoplasia + neonatal seizures + developmental delay = the Hardies-2015 clinical triad that should prompt SLC13A5 sequencing in any neonatal epileptic encephalopathy. This combination is highly specific — fewer than a handful of other genetic epilepsies produce all three features.

**Bone involvement:**
KO mice show reduced cortical bone thickness and compromised mechanical strength. Bone density in DEE25 patients has not been systematically measured — the existing literature attributes growth and bone observations to encephalopathy severity rather than direct NaCT loss in bone. This is a gap.

## Evidence basis

- Source 1: [[research/Dirckx-2022]] — complete mechanistic explanation; ZIP1 cataplerosis; micro-CT human DEE25 teeth; KO mouse dental and bone phenotype.
- Source 2: [[research/Hardies-2015]] — clinical triad as discriminator; dental phenotype first described as DEE25 feature.
- Source 3: [[research/Matricardi-2020]] — tooth hypoplasia as recognizable feature in the natural history cohort.
- Source 4: [[research/Irizarry-2017]] — first report of enamel/bone phenotype in Slc13a5 KO mice.

## Connections to other nodes

- [[T2-CitrateTCAIntegration]] — citrate partitioning in mineralizing cells is the direct metabolic mechanism; the ZIP1 cataplerosis pathway is a tissue-specific variant of the citrate metabolic logic.
- [[T2-ZincCitrateInteraction]] — ZIP1-mediated zinc import is the trigger for the compensatory cataplerosis; the zinc-citrate interaction is central to the paradoxical enamel/bone phenotype.
- [[T1-ExpressionAtlas]] — SLC13A5 expression in osteoblasts and ameloblasts (comparable to testis levels) is documented here; the high expression in mineralizing cells explains why this non-neuronal tissue is affected.

## Open questions

1. Is DXA-measured bone mineral density systematically reduced in DEE25 patients — specifically, do patients have lower bone density than age-matched controls with similar ambulatory status (to control for the effect of immobility on bone density)?
2. Does AAV9/SLC13A5 gene therapy in the mouse model improve bone cortical thickness or mechanical strength when administered before peak osteoblast differentiation — establishing that NaCT restoration can normalize bone phenotype?
3. Is the enamel/dentin phenotype distinguishable from ROGDI-mutation Kohlschütter-Tönz syndrome by micro-CT density analysis — since both syndromes feature amelogenesis imperfecta and the two are commonly confused?
4. Can the tooth micro-CT phenotype (specifically enamel density) serve as a pharmacodynamic biomarker for NaCT activity level in gene therapy trials — if teeth that form after treatment have normalized enamel density, this provides biological evidence of therapeutic NaCT restoration in mineralizing cells?
