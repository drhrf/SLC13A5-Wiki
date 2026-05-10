---
tags: [slc13a5-wiki, tier-2, pathway, liver, lipogenesis, fatty-acid-synthesis, cholesterol, AMPK, metabolic-disease]
tier: 2
node_type: pathway
epistemic_status: established
last_updated: 2026-05-10
linked_nodes:
  - "[[T1-INDYOrthologs]]"
  - "[[T2-CitrateTCAIntegration]]"
  - "[[T2-AcetylCoAProduction]]"
  - "[[T4-MetabolicSyndrome]]"
hypothesis_seeds:
  - "Metformin's NaCT inhibition may contribute to its hepatic lipid-lowering effects independently of complex I — relevant to interpreting metformin trials in NAFLD"
  - "BBB-impermeable NaCT inhibitors could treat NAFLD/T2D without neurological risk — but BBB permeability with aging-related barrier compromise is an underappreciated safety gap"
open_questions:
  - "Does the ~90% reduction in hepatic citrate incorporation into lipids in Slc13a5 KO mice translate quantitatively to humans — or does the higher SLC25A1-mediated mitochondrial citrate export in humans compensate for NaCT loss more effectively?"
  - "Does the SLC13A5-AMPK-PGC1α-mitochondrial biogenesis cascade in KO hepatocytes (Birkenfeld-2011) represent an on-target effect of any NaCT inhibitor — or is it secondary to energy state changes that would differ in partial inhibition vs. complete KO?"
  - "What is the brain exposure of ETG-5773, BI01383298, and Zhang-2024 compound — the three leading NaCT inhibitors — in rodent pharmacokinetic studies?"
---

# Hepatic Lipid Metabolism via Citrate Import

## Core claim

NaCT-mediated citrate import in hepatocytes feeds fatty acid synthesis, cholesterol synthesis, gluconeogenesis, and glycolysis regulation. Loss of hepatic NaCT activity in mice produces a striking metabolic phenotype — 10–17% lower body weight, ~90% reduced hepatic lipogenesis from citrate, reduced hepatic steatosis, and improved insulin sensitivity — through an AMPK-mediated cascade downstream of reduced cytoplasmic citrate. Hepatic SLC13A5 mRNA is upregulated in obese humans with T2D and NAFLD, supporting NaCT inhibition as a therapeutic strategy for metabolic disease. Sources: [[research/Birkenfeld-2011]], [[research/Willmes-2017]], [[research/Kopel-2021]], [[mechanisms/hepatic-citrate-metabolism]].

## Mechanism

The pathway in hepatocytes:

```
Extracellular citrate → NaCT (SLC13A5) → cytoplasmic citrate
    ↓ ACLY
Acetyl-CoA + oxaloacetate
    ↓ ACC1 (acetyl-CoA carboxylase)
Malonyl-CoA → fatty acid synthesis (FAS) → triglycerides, phospholipids
    ↓ HMGCR pathway
Cholesterol synthesis
```

The citrate import also feeds gluconeogenesis (OAA → PEPCK → PEP → glucose) and inhibits glycolysis allosterically (citrate is an allosteric inhibitor of phosphofructokinase/PFK).

**AMPK cascade (✅ Established by Birkenfeld-2011):**
Reduced citrate import → lower cytoplasmic citrate → reduced ATP/ADP ratio (measured by 31P-NMR in KO hepatocytes) → AMPK activation → dual downstream effects:
1. AMPK phosphorylates/inactivates ACC-2 → reduced malonyl-CoA → disinhibited CPT1 → increased mitochondrial fatty acid import and β-oxidation
2. AMPK activates PGC-1α → mitochondrial biogenesis → increased OXPHOS capacity
3. Reduced SREBP-1c → reduced transcription of lipogenic enzymes (FAS, ACC1, SCD1)

Net effect: hepatocytes switch from lipogenesis to lipid oxidation, producing the metabolically protected phenotype.

**Metformin-NaCT connection (✅ Established by Kopel-2020):**
Metformin directly inhibits NaCT in hepatocytes, independently of its established complex I (respiratory chain) mechanism. Inhibition of NaCT by metformin → reduced intracellular citrate → reduced ACLY activity → reduced lipogenesis → reduced allosteric citrate inhibition of PFK → increased glycolysis. This adds a second mechanism to metformin's hepatic action. Clinical implication: SLC13A5 heterozygous carriers on metformin may have citrate transport reduced below a threshold relevant to neurological effects, particularly in brain under stress conditions.

**Species translation caveat:** The mouse Slc13a5 KO produces ~90% reduction in hepatic citrate incorporation into lipids. Human SLC13A5 has markedly higher transport capacity (Vmax). Quantitative translation to humans requires caution — pharmacological inhibition in humans may need to achieve much deeper inhibition than genetic KO in mice to produce comparable lipogenic suppression.

**NaCT inhibitor landscape (current):**
- Compound 2 (PF-06649298): substrate-competitive; Pfizer; brain exposure unstated (critical safety gap).
- ETG-5773: non-competitive, cross-species active; reduces hepatic steatosis in DIO mice — first pharmacological confirmation that NaCT inhibition (not just genetic KO) improves liver fat.
- BI01383298: IC₅₀ 25 nM; >1000-fold selective over NaDC1/NaDC3; SGC chemical probe.
- Zhang-2024 compound: IC₅₀ 67 nM.

## Evidence basis

- Source 1: [[research/Birkenfeld-2011]] — foundational; mINDY KO metabolic phenotype; AMPK cascade; kinetics; lipogenesis and insulin sensitivity data.
- Source 2: [[research/Willmes-2017]] — mINDY upregulated in human NAFLD/T2D liver; mammals/humans connection.
- Source 3: [[research/Kopel-2021]] — comprehensive review; hepatocyte citrate function; liver vs. neuron distinction; safety argument.
- Source 4: [[research/Kopel-2020]] — metformin as direct NaCT inhibitor; clinical safety implications.
- Source 5: [[research/Zahn-2022]] — ETG-5773 pharmacological NaCT inhibition rescues hepatic steatosis in vivo.
- Source 6: [[research/Quigley-2026]] — BI01383298 as SGC chemical probe with >1000-fold NaDC selectivity.
- Source 7: [[mechanisms/hepatic-citrate-metabolism]] — comprehensive mechanism review.

## Connections to other nodes

- [[T1-INDYOrthologs]] — the Drosophila INDY and mouse mINDY KO data that established the hepatic metabolic protection phenotype; the ortholog history provides context for the human therapeutic logic.
- [[T2-CitrateTCAIntegration]] — hepatic citrate sits at the same TCA branch point as neuronal citrate; the downstream consequences differ by cell type.
- [[T2-AcetylCoAProduction]] — ACLY is the shared enzyme in hepatocytes and neurons; in liver it produces acetyl-CoA for lipid synthesis rather than ACh.
- [[T4-MetabolicSyndrome]] — this is the therapeutic side: NaCT inhibition for NAFLD, obesity, T2D; the Tier 4 node captures the clinical translation.

## Open questions

1. What is the brain exposure of ETG-5773, BI01383298, and the Zhang-2024 compound in rodent pharmacokinetic studies — the single most important safety question for any NaCT inhibitor program targeting metabolic disease?
2. Does the AMPK-PGC1α mitochondrial biogenesis cascade (downstream of NaCT inhibition in hepatocytes) produce any hepatic co-expression of SLC13A5-module genes (as identified by Ferreira-2026 in brain) — suggesting conserved mitochondrial biogenesis regulation across tissues?
3. Can a partial NaCT inhibitor (targeting 50% rather than 100% of activity) achieve therapeutically meaningful lipogenesis reduction without the full metabolic-protection phenotype of complete KO — relevant to finding a therapeutic window that avoids potential neurological effects in older patients?
4. In humans on metformin who are SLC13A5 heterozygous carriers (reduced transport capacity at baseline), are plasma or CSF citrate levels elevated to a degree that suggests combined metformin + heterozygosity brings transport below the threshold that matters neurologically?
