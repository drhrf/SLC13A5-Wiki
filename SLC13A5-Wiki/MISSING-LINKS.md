---
tags: [slc13a5-wiki, maintenance, missing-links, wikilinks, broken-references]
node_type: maintenance
last_updated: 2026-05-10
---

# Missing Links Register

This file tracks wikilinks in wiki nodes that point to targets not yet created as wiki nodes. Each entry records: the linking node, the unresolved target, what the target should cover, and whether it is a high priority to create.

---

## Category 1 — Research paper nodes cited but not created as wiki nodes

These are wikilinks in the format `[[research/PAPER-YEAR]]` that reference vault research notes (which exist in `/SLC13A5/research/`) but have not been converted to wiki nodes. The wiki uses these as source citations rather than as standalone nodes, which is acceptable. No action required unless the paper is a primary evidence source for a top-10 gap.

| Wikilink target | Cited in node(s) | Vault source exists? | Priority |
|----------------|-----------------|----------------------|----------|
| [[research/Bainbridge-2017]] | T3-UrinaryMetabolomicsSignature, EDGE-MAP | Yes | Low |
| [[research/Birkenfeld-2011]] | T2-HepaticLipidMetabolism, T4-MetabolicSyndrome | Yes | Low |
| [[research/Fan-2021]] | T1-INDYOrthologs, T4-AlzheimerDisease | Yes | Low |
| [[research/Ferreira-2026]] | T1-ExpressionAtlas, T2-MitochondrialBioenergetics | Yes | Low |
| [[research/Gul-Hinc-2026]] | T2-AcetylCoAProduction, T4-AlzheimerDisease | Yes | Low |
| [[research/Pourshafie-2026]] | T2-AcetylCoAProduction, T2-HistoneAcetylation | Yes | Low |
| [[research/Wang-2025]] | T1-VariantCatalog, T3-UrinaryMetabolomicsSignature | Yes | Low |
| [[research/Bailey-2026]] | T3-NeonatalEpilepsy | Yes | Low |
| [[research/Dirckx-2022]] | T3-ToothEnamelHypoplasia, T2-ZincCitrateInteraction | Yes | Low |
| [[research/Kumar-2021]] | T2-CitrateTCAIntegration, T4-CancerMetabolism | Yes | Low |
| [[research/Klotz-2016]] | CONTESTED-CLAIMS, T3-NeonatalEpilepsy | Yes | Low |
| [[research/Matricardi-2020]] | T3-NeonatalEpilepsy, T3-IntellectualDisability | Yes | Low |
| [[research/Jaramillo-Martinez-2024]] | T1-VariantCatalog | Yes | Low |
| [[research/Lin-2021]] | T3-UrinaryMetabolomicsSignature, T4-AlzheimerDisease | Yes | Low |
| [[research/Tremblay-Franco-2024]] | T4-AlzheimerDisease | Yes | Low |
| [[research/Hofling-2026]] | T4-AlzheimerDisease, CONTESTED-CLAIMS | Yes | Low |
| [[research/Willmes-2017]] | T4-MetabolicSyndrome, T1-INDYOrthologs | Yes | Low |
| [[research/Lal-2026]] | T3-UrinaryMetabolomicsSignature | Yes | Low |
| [[research/Brown-Nye-Porter-2021]] | T3-MovementAbnormalities, T3-HepaticMetabolicPhenotype | Yes | Low |
| [[research/Alsemari-2023]] | T3-MovementAbnormalities | Yes | Low |
| [[research/Milosavljevic-2022]] | T3-UrinaryMetabolomicsSignature | Yes | Low |
| [[research/Zahn-2022]] | T4-MetabolicSyndrome | Yes | Low |
| [[research/Quigley-2026]] | T4-MetabolicSyndrome | Yes | Low |
| [[research/Ozlu-2025]] | T3-NeonatalEpilepsy | Yes | Low |
| [[research/Ozlu-2024]] | T3-IntellectualDisability | Yes | Low |

---

## Category 2 — Mechanism/condition nodes cited in wiki but not created

These are wikilinks targeting mechanism or condition notes in the original vault (not wiki nodes). They function as cross-references to the source vault and are generally acceptable. No resolution required unless the concept warrants its own wiki node.

| Wikilink target | Cited in node(s) | Should become a wiki node? |
|----------------|-----------------|---------------------------|
| [[conditions/SLC13A5-deficiency]] | T3-NeonatalEpilepsy, T3-IntellectualDisability | No — vault hub file, referenced appropriately |
| [[genes/SLC13A5]] | T1-SLC13A5-GeneStructure | No — vault gene file |
| [[mechanisms/acetyl-CoA-neurodegeneration]] | T2-AcetylCoAProduction | No — vault mechanism file |
| [[mechanisms/hepatic-citrate-metabolism]] | T4-CancerMetabolism | No — vault mechanism file |

---

## Category 3 — Cross-wiki links with no corresponding node (HIGH PRIORITY)

These are wikilinks in the format `[[T*-*]]` that point to wiki nodes that should exist but do not yet.

| Wikilink target | Cited in node(s) | Target description | Priority | Status |
|----------------|-----------------|-------------------|----------|--------|
| None identified | — | All T1–T4 node cross-links resolve to created files | — | ✅ All resolved |

*Note: As of 2026-05-10, all [[T1-]], [[T2-]], [[T3-]], and [[T4-]] wikilinks created in this wiki session resolve to existing wiki nodes. No broken intra-wiki links identified.*

---

## Category 4 — Claimed vault sources that require verification

These are citations in wiki nodes where the vault source was identified from memory or cross-reference rather than direct confirmation of the source file's content. They should be verified before any manuscript submission.

| Claimed citation | Cited in node | Claim made | Verification needed |
|-----------------|--------------|------------|---------------------|
| Rigby-2022 | T3-MovementAbnormalities, T2-AcetylCoAProduction | Neuron-specific SLC13A5 overexpression produces white matter disruption | Verify: does vault/research/Rigby-2022.md confirm white matter finding? |
| Henke-2020 | T4-AlzheimerDisease (queries file) | Hippocampal hyperexcitability in Slc13a5 KO mice | Verify in vault/research/ |
| He-2025 | T1-SLC13A5-Protein (via VariantCatalog) | Structural data | Verify citation details |
| Sauer-2021 | T1-SLC13A5-Protein | Cryo-EM structure 3.04 Å / 7JSK | Verify PDB accession |
| Li-Wang-2021 | T2-TranscriptionalRegulation | Highest hepatic expression; regulatory overview | Verify distinction from Li-2021-PXR |
| Duan-2021 | T1-VariantCatalog | CNV-class variants in DEE25 | Verify vault file content |

---

## Category 5 — Speculative or cross-domain claims flagged as needing primary literature verification

These are noted explicitly in wiki nodes as requiring verification but do not correspond to vault sources. They require a targeted literature search before the claims can be elevated above 💡 Speculative.

| Claim | Node | Status |
|-------|------|--------|
| Direct citrate → mTOR lysosomal sensing mechanism (independent of AMPK) | T2-mTORSignaling | 💡 No vault source — cross-domain inference |
| SLC13A5 in oligodendrocytes during myelination | T3-MovementAbnormalities | 💡 Not confirmed in vault; requires Allen Cell Atlas query |
| Warburg effect + reductive carboxylation in HCC + NaCT-imported citrate interchangeability | T4-CancerMetabolism | 💡 Mechanistic inference from cancer metabolism literature |
| Histone acetylation in SLC13A5-deficient neurons at synaptic gene loci | T2-HistoneAcetylation | 💡 No vault source — cross-domain from Pourshafie-2026 (ACSS2) |
| AMPK → mTORC1 suppression in NaCT-deficient neurons (not measured in Birkenfeld-2011 neurons; only hepatocytes) | T2-mTORSignaling | 💡 Extrapolation from hepatocyte data |

---

## Maintenance schedule

This file should be updated whenever:
- A new wiki node is created (check whether any existing missing-link entries are now resolved)
- A new wikilink is added to an existing node (check whether the target exists)
- A claimed citation is verified (move from Category 4 to Category 1 with "vault source exists: Yes")

Last full audit: 2026-05-10.
