---
tags: [slc13a5-wiki, tier-2, pathway, mTOR, lysosomal, nutrient-sensing, autophagy, citrate]
tier: 2
node_type: pathway
epistemic_status: speculative
last_updated: 2026-05-10
linked_nodes:
  - "[[T2-CitrateTCAIntegration]]"
  - "[[T2-AcetylCoAProduction]]"
  - "[[T2-MitochondrialBioenergetics]]"
  - "[[T4-MetabolicSyndrome]]"
hypothesis_seeds:
  - "Reduced cytoplasmic citrate in SLC13A5-deficient neurons signals reduced nutrient availability to mTORC1, mimicking dietary restriction and explaining the Fan-2021 cognitive benefit of brain NaCT reduction in adult mice"
  - "Lysosomal citrate sensing via a yet-uncharacterized sensor could link NaCT activity to mTORC1 regulation in neurons — a mechanism analogous to the lysosomal amino acid sensing that controls mTORC1 through Ragulator-Rag"
open_questions:
  - "Does NaCT loss in neurons reduce mTORC1 activity in a citrate-concentration-dependent manner — measurable by phospho-S6K1 and phospho-4EBP1 in SLC13A5-deficient iPSC neurons vs. controls?"
  - "Is there a lysosomal citrate transporter analogous to SLC25A1 that exports citrate from lysosomes to the cytoplasm — and does NaCT-derived citrate feed this lysosomal pool?"
  - "Does the AMPK activation observed in Slc13a5 KO hepatocytes (Birkenfeld-2011) include secondary mTORC1 suppression via the AMPK-TSC2-Rheb pathway — and is this also present in neurons?"
---

# mTOR Signaling and Citrate

## Core claim

mTOR complex 1 (mTORC1) is a master nutrient sensor that integrates signals from amino acids, glucose, lipids, and energy charge to regulate protein synthesis, autophagy, and cell growth. Citrate, as a central TCA cycle intermediate and energy-status indicator, is a plausible upstream input to mTORC1 signaling. NaCT-mediated citrate import may influence mTORC1 activity in neurons by modulating the cytoplasmic citrate concentration and the ATP/ADP ratio that is sensed by AMPK — an upstream mTORC1 inhibitor. This connection is speculative and not directly demonstrated in SLC13A5 biology; it is mechanistically motivated by established AMPK-mTOR crosstalk and by the dietary-restriction-mimetic phenotype of mINDY knockouts. Sources: [[research/Birkenfeld-2011]], [[research/Fan-2021]], [[research/Kopel-2021]]; mTOR-citrate connection: No vault source directly demonstrates mTOR modulation by NaCT activity. Claim derived from cross-domain inference. Requires primary literature verification.

## Mechanism

**mTORC1 activation pathway (✅ Established — not in SLC13A5 context):**
mTORC1 is recruited to the lysosomal surface by the Ragulator-Rag GTPase complex in response to amino acid sufficiency. On the lysosome, mTORC1 is activated by Rheb-GTP (controlled by TSC1/TSC2 GTPase activating complex, itself downstream of growth factor and energy signals). Active mTORC1 phosphorylates S6K1 and 4EBP1, promoting translation and inhibiting autophagy.

**AMPK-mTOR axis (✅ Established — relevant via Birkenfeld-2011 hepatocyte data):**
AMPK (AMP-activated protein kinase) is activated by elevated AMP/ATP ratio (reduced energy charge). Active AMPK inhibits mTORC1 by: (1) phosphorylating TSC2, stabilizing the TSC1/2 complex → increased Rheb-GTP hydrolysis → less Rheb-GTP → reduced mTORC1 activation; (2) directly phosphorylating Raptor (mTORC1 component).

In Slc13a5 KO hepatocytes (Birkenfeld-2011), NaCT loss → reduced cytoplasmic citrate → reduced ATP/ADP ratio (measured by 31P-NMR) → AMPK activation. The secondary mTORC1 suppression was not measured in that study, but follows directly from established AMPK signaling logic.

**Citrate as direct mTOR input (💡 Speculative):**
The lysosomal sensing machinery for mTORC1 has been most extensively characterized for amino acids. A citrate-specific lysosomal sensing mechanism has been proposed in the metabolic literature (lysosomal citrate export and mTOR activation). Whether a direct citrate → mTOR signaling axis exists independent of AMPK is not established in the vault. No vault source confirms this.

**Dietary restriction connection (🔶 Emerging):**
Dietary restriction (DR) — which extends lifespan and improves cognition in rodents — suppresses mTORC1. The mINDY KO metabolic phenotype (Birkenfeld-2011) and the brain-specific mINDY deletion cognitive benefit (Fan-2021) both phenocopy DR. If the mechanism of DR mimicry in mINDY KO is AMPK-mTORC1 suppression via reduced citrate-derived ATP, this would place NaCT activity directly upstream of the mTOR pathway in the DR-lifespan axis — a testable hypothesis.

**Autophagy connection:**
mTORC1 suppression promotes autophagy. In neurons, autophagy is essential for clearing misfolded proteins (tau, α-synuclein). If reduced NaCT activity → AMPK → mTORC1 suppression → increased autophagy, this could be a neuroprotective mechanism — explaining the Fan-2021 cognitive benefit of NaCT reduction in adult mice. Conversely, in developing brain where protein synthesis is essential for circuit formation, mTORC1 suppression from NaCT loss could impair the protein synthesis needed for synaptogenesis.

## Evidence basis

- Source 1: [[research/Birkenfeld-2011]] — AMPK activation in NaCT-deficient hepatocytes; reduced ATP/ADP ratio; mechanistic starting point for the AMPK-mTOR chain.
- Source 2: [[research/Fan-2021]] — DR-mimetic cognitive benefit from brain NaCT reduction; consistent with mTORC1 suppression as a downstream mechanism but not directly measured.
- Source 3: [[research/Kopel-2021]] — caloric restriction mimicry in mINDY biology; DR connection reviewed.
- Source 4: Direct citrate → mTOR signaling — No vault source. Claim derived from cross-domain inference from the broader mTOR literature. Requires primary literature verification.

## Connections to other nodes

- [[T2-CitrateTCAIntegration]] — the cytoplasmic citrate pool is the upstream variable; reduced citrate from NaCT loss changes ATP/ADP ratio which feeds AMPK-mTOR.
- [[T2-AcetylCoAProduction]] — mTOR regulates translation of metabolic enzymes including ACLY; mTOR suppression could feed back to reduce ACLY expression.
- [[T2-MitochondrialBioenergetics]] — AMPK activates PGC-1α and mitochondrial biogenesis; the NaCT-AMPK-mTOR axis is mechanistically intertwined with the bioenergetics node.
- [[T4-MetabolicSyndrome]] — in hepatocytes, NaCT-AMPK-mTOR suppression may contribute to the metabolic protection phenotype; mTOR inhibition reduces hepatic lipogenesis (SREBP-1c is a downstream mTOR target).

## Open questions

1. Does SLC13A5 loss in iPSC-derived neurons (DEE25 patient-derived or CRISPR-engineered) reduce phospho-S6K1 and phospho-4EBP1 levels relative to isogenic controls — indicating mTORC1 suppression? This is the most direct cell-autonomous test.
2. Does the AMPK activation in Slc13a5 KO hepatocytes (measured by Birkenfeld-2011) extend to secondary mTORC1 suppression — measurable by raptor phosphorylation, ULK1 activation (autophagy initiation), and p62/LC3 autophagic flux?
3. Does mTORC1 suppression mediate the Fan-2021 cognitive benefit — specifically, does rapamycin (mTORC1 inhibitor) in WT mice produce a similar cognitive phenotype to brain-specific mINDY deletion, and does AICAR (AMPK activator) phenocopy mINDY deletion without metabolic manipulation?
4. Is mTORC1 hyperactivated in SLC13A5-deficient neonatal neurons — due to the paradoxical accumulation of extracellular citrate (which cannot be imported) providing amino acid-like nutrient signals to the lysosomal sensing machinery, or due to downstream metabolic changes that signal nutrient excess to mTOR?
