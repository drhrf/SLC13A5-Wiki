---
tags: [slc13a5-wiki, tier-3, phenotype, epilepsy, seizure, neonatal, EEG, DEE25]
tier: 3
node_type: phenotype
epistemic_status: established
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-GABAMetabolism]]"
  - "[[T2-NMDAModulation]]"
  - "[[T2-Anaplerosis]]"
  - "[[T2-CitrateTCAIntegration]]"
  - "[[T3-IntellectualDisability]]"
  - "[[T3-MovementAbnormalities]]"
hypothesis_seeds:
  - "The spontaneous age-related seizure remission in DEE25 parallels the declining cerebrum SLC13A5 expression trajectory — suggesting that reduced NaCT expression in older patients normalizes the excitatory-inhibitory imbalance that peaked during infancy"
  - "Acetazolamide benefit (Klotz-2016, 4/9 responders) may operate via carbonic anhydrase inhibition in GABAergic interneurons, specifically restoring the inhibitory function that NaCT loss impairs"
open_questions:
  - "Is the spontaneous seizure remission in DEE25 mechanistically linked to declining SLC13A5 expression — or to compensatory KCC2 upregulation, myelination maturation, or other developmental processes independent of NaCT?"
  - "What EEG pattern (focal, multifocal, generalized) is most specific to DEE25 among early-onset epileptic encephalopathies — and does the pattern correlate with the high-SLC13A5-expression brain regions at seizure onset?"
  - "Why does acetazolamide help ~4/9 patients but not others — what clinical or genetic variables predict response?"
---

# Neonatal Epilepsy

## Core claim

Clonic or tonic seizures presenting in the first days of life are the universal presenting feature of SLC13A5 deficiency, occurring in essentially all reported patients. Seizure burden is highest in the first three years and declines with age, with most adults being seizure-free or near seizure-free — a trajectory that parallels but does not mechanistically equal the declining SLC13A5 cerebrum expression after the first postnatal year. The primary mechanistic hypothesis is GABA synthesis impairment, supported by the pharmacological effectiveness of GABA-system drugs. Ketogenic diet is contraindicated (worsens symptoms in Klotz-2016). Sources: [[conditions/SLC13A5-deficiency]], [[research/Matricardi-2020]], [[research/Klotz-2016]], [[research/Ozlu-2025]], [[research/Ozlu-2024]], [[research/Bailey-2026]].

## Mechanism

The leading mechanistic explanation for neonatal onset: NaCT-mediated citrate import in developing neurons is essential for maintaining GABA synthesis precursor flux. Loss of NaCT → reduced cytoplasmic citrate → reduced TCA anaplerosis → reduced glutamate → reduced GABA → impaired GABAergic inhibition → network hyperexcitability → seizures (see [[T2-GABAMetabolism]] for full pathway).

Additional contributions: extracellular citrate accumulation (NaCT cannot clear it) → zinc chelation → altered NMDA modulation → changed excitatory tone (see [[T2-NMDAModulation]]).

**Developmental trajectory of seizure burden (✅ Established — Matricardi-2020, n=14):**

| Age epoch | Seizure-free rate |
|-----------|-----------------|
| 0–3 years | 14% |
| 3–12 years | 60% |
| 12–18 years | 57% |
| >18 years | 100% (n=3 only; very limited) |

Seizure type: clonic or tonic at onset; 57% evolve to status epilepticus. Fever commonly triggers seizures. Most EEGs are abnormal but fewer than one-third have frequent interictal epileptiform activity (Ozlu-2025) — suggesting that IEA is not the primary driver of neurocognitive dysfunction, which persists even when seizure activity decreases.

**Most effective anti-seizure medications (✅ Established from cohort data):**
- Valproic acid: most widely used (22/30 in Ozlu-2025); 80% caregiver report of benefit; GABA-transaminase inhibitor
- Benzodiazepines: GABAergic; effective particularly in acute seizure management
- Phenobarbital: GABAergic; also PXR agonist (upregulates hepatic SLC13A5 — clinical relevance uncertain in biallelic LoF)
- Phenytoin: Na+ channel; adjunctive
- Carbamazepine: Na+ channel; dramatic efficacy in one severe burst-suppression case (Santalucia-2022)
- Acetazolamide: carbonic anhydrase inhibitor; reduced seizures in 4/9 patients in Klotz-2016; mechanism in DEE25 not established; only novel pharmacology hit in the vault

**Contraindicated:** Ketogenic diet and fasting (worsened in Klotz-2016) — critical clinical alert; contradicts standard pediatric epilepsy practice.

**Gene therapy rescue of seizure phenotype (✅ Preclinical — Bailey-2026):**
AAV9/SLC13A5 via ICM or IT injection in Slc13a5 KO mice normalized EEG epileptiform activity, restored seizure resistance to chemically induced challenge, and showed efficacy at both neonatal (P10) and young adult treatment windows. ICM delivery outperformed IT for brain transduction. This provides the first preclinical proof-of-concept for disease-modifying therapy.

## Evidence basis

- Source 1: [[research/Matricardi-2020]] — age-stratified seizure remission data; natural history; n=14.
- Source 2: [[research/Klotz-2016]] — variant characterization cohort; ketogenic diet warning; acetazolamide benefit; anti-seizure medication effectiveness.
- Source 3: [[research/Ozlu-2025]] — prospective natural history (n=30, 2-year follow-up); ASM use; caregiver-reported outcomes; EEG analysis.
- Source 4: [[research/Ozlu-2024]] — longitudinal cognitive and developmental outcomes.
- Source 5: [[research/Bailey-2026]] — preclinical gene therapy rescue of seizure phenotype.
- Source 6: [[research/Santalucia-2022]] — carbamazepine efficacy in severe burst-suppression case.

## Connections to other nodes

- [[T2-GABAMetabolism]] — primary mechanistic explanation for seizure onset; GABA synthesis impairment from reduced citrate precursor flux.
- [[T2-NMDAModulation]] — secondary mechanism; extracellular citrate accumulation modulates zinc and NMDA receptor function.
- [[T2-Anaplerosis]] — why ketogenic diet worsens DEE25; failed compensation from anaplerotic substrate shift.
- [[T2-CitrateTCAIntegration]] — the TCA perturbation signature (Bainbridge-2017) as the biochemical context for seizure pathophysiology.
- [[T3-IntellectualDisability]] — seizure burden decreases with age while intellectual disability does not; the dissociation of these two outcomes is a key clinical observation requiring mechanistic explanation.
- [[T3-MovementAbnormalities]] — motor impairment co-occurs with seizures, particularly in the neonatal period; the two phenotypes are partially dissociable.

## Open questions

1. Is the spontaneous seizure remission trajectory (14% seizure-free at 0–3 years → 100% at >18 years) causally linked to declining SLC13A5 expression — or are other developmental changes (KCC2 maturation, myelination, axonal pruning) the primary drivers of remission? An experiment: do DEE25 patients with faster SLC13A5 expression decline (if measurable via accessible blood or CSF biomarkers) show earlier seizure remission?
2. What is the mechanism of acetazolamide benefit in the ~44% of DEE25 patients who respond — is it via neuronal intracellular pH, carbonic anhydrase in GABAergic interneurons, or another route? Metabolomic profiling before and after acetazolamide in responders vs. non-responders could reveal the pharmacodynamic target.
3. Does the EEG ictal onset zone in DEE25 preferentially involve hippocampus and temporal cortex — the high-SLC13A5-expressing regions at the postnatal peak per the regional expression hypothesis (H5 in [[queries/hypotheses-SLC13A5-developmental-disorders]])?
4. At what minimal degree of NaCT restoration (e.g., 10%, 20%, 50% of WT transport capacity) does the epileptic phenotype normalize in the mouse model — establishing the therapeutic threshold for gene therapy?
