# Structured Epistemic Knowledge Graph — Framework Specification

**Version:** 1.0  
**Date:** 2026-05-10  
**Reference paper:** Freitas HR et al. "A structured epistemic knowledge graph for hypothesis generation in rare disease research: proof of concept in SLC13A5 citrate transporter disorder (DEE25)." *Orphanet Journal of Rare Diseases* (under review).  
**Repository:** [GITHUB URL]  
**Zenodo DOI:** [DOI — assigned at v1.0 release]  
**License:** CC-BY 4.0

---

## Purpose

This document specifies a reusable framework for structured evidence synthesis and hypothesis generation in rare disease research. It is designed for situations where:

- A gene is implicated in a severe rare condition but the evidence base is thin, heterogeneous, and dispersed across molecular biology, pathway physiology, clinical phenotyping, and adjacent disease fields.
- The evidence is insufficient for formal systematic review or meta-analysis but too complex for reliable informal expert synthesis.
- The goal is to surface testable hypotheses and identify the experiments most likely to advance the field, not to produce a narrative review.

The framework organizes evidence into a four-tier directed graph of typed nodes. Every claim within a node carries an explicit epistemic label. Mechanistic connections between nodes are documented as typed edges, with confirmed and inferred edges recorded separately. Hypotheses generated from the graph are classified by prior probability and assigned a testability criterion. Internal contradictions are registered explicitly rather than suppressed.

The SLC13A5/DEE25 wiki in this repository is the proof-of-concept application of this framework. The specification below is domain-agnostic and can be applied to any under-characterized gene in any rare disease.

---

## Repository structure

A repository implementing this framework should follow this layout:

```
repository-root/
│
├── README.md                  ← what this is, how to cite, DOI
├── FRAMEWORK-SPEC.md          ← this document
│
├── [GENE]-Wiki/               ← the gene-specific wiki (replace [GENE])
│   ├── 00-INDEX.md            ← master node index with Mermaid graph
│   ├── EDGE-MAP.md            ← all confirmed and inferred edges
│   ├── HYPOTHESES.md          ← hypothesis registry (all tiers)
│   ├── RESEARCH-AGENDA.md     ← prioritized studies by time horizon
│   ├── MISSING-LINKS.md       ← broken wikilinks and unverified citations
│   │
│   ├── Tier1-Molecular/       ← molecular identity nodes
│   ├── Tier2-Pathways/        ← pathway and metabolic context nodes
│   │   └── CONTESTED-CLAIMS.md ← internal contradiction register
│   ├── Tier3-Phenotypes/      ← clinical and organismal phenotype nodes
│   └── Tier4-DiseaseConnections/ ← adjacent disease hypothesis nodes
│
└── edge-map.csv               ← machine-readable adjacency list (generated)
```

Obsidian is the recommended editing environment because it renders wikilinks, displays the graph view, and handles the YAML frontmatter used in this framework. The Markdown files are plain text and readable in any environment; Obsidian is not required for consumers of the archive.

---

## Tier definitions

### Tier 1 — Molecular identity

**Scope:** What the gene product is, how it works, and what is directly known about its sequence, structure, expression, and variants.

**Inclusion criteria:** Claims that can be attributed to primary structural, biochemical, or cell-biological experiments on the gene product itself. Expression data, kinetic parameters, structural features, variant classifications, post-translational modifications, and protein-protein interaction data. Species orthologs and their comparative properties.

**Exclusion criteria:** Downstream pathway effects (Tier 2). Clinical consequences (Tier 3). Connections to adjacent diseases (Tier 4).

**Typical node count:** 5–12 nodes depending on how well-characterized the gene is.

**Example nodes (SLC13A5):** protein structure and transport mechanism; expression pattern; variant classification; species orthologs; protein interactome; deep mutational scanning.

---

### Tier 2 — Pathways and metabolic context

**Scope:** How the gene product participates in cellular metabolic or signaling pathways, and what happens to those pathways when the gene is lost or overactive.

**Inclusion criteria:** Pathway membership (KEGG, Reactome, or primary literature). Metabolic flux effects. Anaplerotic or cataplerotic roles. Co-expression modules. Upstream regulators and downstream effectors with at least one cited mechanistic link. Therapeutic interventions that target the pathway.

**Exclusion criteria:** Whole-organism or tissue-level phenotypes (Tier 3). Connections to diseases other than the primary rare disease (Tier 4).

**Typical node count:** 6–14 nodes.

**Example nodes (SLC13A5):** TCA cycle anaplerosis; hepatic lipid metabolism; cholinergic neurotransmission; histone acetylation and epigenetic regulation; contested claims register.

**Note:** The contested claims register lives in Tier 2 because most internal contradictions in rare disease evidence arise from mechanistic interpretation disagreements. It is a synthesis file, not a node, and does not carry a tier label in its frontmatter.

---

### Tier 3 — Phenotypes

**Scope:** The clinical, cellular, organismal, and biofluid phenotypes associated with loss or gain of the gene product, in both the primary rare disease and relevant animal models.

**Inclusion criteria:** Documented clinical phenotypes in human patients. Animal model phenotypes with mechanistic links back to Tier 1 or Tier 2. Biomarker profiles in patients or models. Genotype-phenotype correlations. Treatment response data (including null responses and adverse effects).

**Exclusion criteria:** Phenotypes in adjacent diseases where the gene's causal role is hypothetical (Tier 4). Purely molecular readouts without clinical or organismal manifestation (Tier 2).

**Typical node count:** 4–10 nodes.

**Example nodes (SLC13A5):** neonatal epilepsy; intellectual disability and cognitive phenotype; dental enamel hypoplasia; hepatic and metabolic phenotype; biofluid metabolite panel.

---

### Tier 4 — Disease connections

**Scope:** Adjacent or downstream diseases in which the gene product is a biologically motivated but unconfirmed candidate. This tier is explicitly speculative by design; it exists to make speculative connections visible, evidenced, and testable rather than leaving them in informal expert conversation.

**Inclusion criteria:** A mechanistic chain — however partial — connecting Tier 1 or Tier 2 biology to the adjacent disease. At least one cited piece of evidence (co-expression, biomarker, genetic association, or model data) for the connection. A clearly stated falsification criterion.

**Exclusion criteria:** Connections that rely solely on the gene being in a pathway with known disease involvement, with no gene-specific evidence. These belong in the open questions of a Tier 2 node, not in a Tier 4 node of their own.

**Typical node count:** 2–6 nodes. More than six Tier 4 nodes is a signal that the speculative scope is too broad.

**Example nodes (SLC13A5):** Alzheimer's disease; metabolic syndrome; neurodegeneration broadly; cancer metabolism.

---

## Epistemic labeling protocol

Every substantive claim in every node file carries one of four epistemic labels. Labels are assigned at the claim level, not at the node level. A single node file will typically contain claims carrying two or three different labels.

---

### ✅ Established

**Criterion:** The claim is supported by at least two independent primary studies using different methods, or by one study with very large sample size and replication in a secondary analysis, and no credible contrary evidence exists in the literature.

**Decision rule:** Ask: "Would a reviewer for a top-tier journal in this field accept this claim without a citation?" If yes, it is Established. If the citation is necessary, apply the Emerging criterion instead.

**Worked example (SLC13A5):** "SLC13A5 encodes a sodium-coupled citrate transporter that co-transports 3 Na+ per citrate3- (electrogenic)." This is established by independent functional expression studies in Xenopus oocytes and mammalian cell lines, confirmed in the cryo-EM structure. ✅ Established.

---

### 🔶 Emerging

**Criterion:** The claim is supported by at least one primary study with adequate methodology, but has not been independently replicated, or the replication used a different system that raises translation questions, or the sample size is small (n < 30 for human data).

**Decision rule:** Ask: "Is this finding real but fragile — would a single contradicting study materially weaken it?" If yes, it is Emerging.

**Worked example (SLC13A5):** "Acetazolamide reduced seizures in 4 of 9 DEE25 patients (Klotz-2016)." One study, n=9, retrospective, no controls. The signal is real but a single negative replication would substantially change the assessment. 🔶 Emerging.

---

### 💡 Speculative

**Criterion:** The claim is mechanistically motivated and internally coherent, but rests on inference from studies in different systems, developmental stages, or species, with no direct measurement of the claimed connection in the relevant context.

**Decision rule:** Ask: "Could someone publish a paper specifically testing this claim, with a reasonable expectation of a novel finding?" If yes, it is Speculative (testable novelty). If the claim is so vague that no specific test can be designed, it should not be a claim at all.

**Worked example (SLC13A5):** "NaCT loss in DEE25 neurons reduces acetyl-CoA availability for histone acetylation, contributing to irreversible cognitive deficits." The ACLY-acetyl-CoA-histone acetylation chain is established. The NaCT-ACLY connection is established. But no study has measured histone acetylation in NaCT-deficient human neurons. The inference is coherent, the test is designable, the claim is speculative. 💡 Speculative.

---

### ❓ Unknown

**Criterion:** The claim involves a comparison or measurement that has not been made, or where the available studies do not address the relevant question directly (e.g., studies exist in a related population or condition but not in the one under examination).

**Decision rule:** Ask: "Is the reason we don't know this that no one has looked, rather than that the evidence is mixed?" If yes, it is Unknown.

**Worked example (SLC13A5):** Whether CSF citrate is reduced in Alzheimer's disease relative to age-matched cognitively normal controls. Studies measure CSF citrate in aging normals (Lin-2021) and in neurological disease comparisons (Hofling-2026), but the specific AD-vs-normal comparison is not in any available study. ❓ Unknown.

---

### Boundary cases and the contested claims register

When two credible studies point in opposite directions, do not average them into a single label. Register the contradiction explicitly in the Contested Claims Register (CONTESTED-CLAIMS.md) with both sources, the mechanism-level reasoning for each direction, and the evidence that would resolve the disagreement. In the node files that reference the contested claim, use the label of the claim as it stands in the primary source most relevant to the node's argument, and add a wikilink to the contested claims entry: `[CONTESTED-CLAIMS CC1]`.

---

## Node file template

Every node file (Tier 1 through Tier 4) uses the following Markdown structure:

```markdown
---
tags: [gene-wiki, tier-label, topic-tags]
node_type: [molecular | pathway | phenotype | disease-connection]
tier: [1 | 2 | 3 | 4]
epistemic_status: [established | emerging | speculative | unknown | mixed]
last_updated: YYYY-MM-DD
linked_nodes:
  - "[[NodeID1]]"
  - "[[NodeID2]]"
hypothesis_seeds:
  - "Brief statement of a testable hypothesis that could be built from this node"
open_questions:
  - "A specific knowledge gap directly motivated by this node's content"
---

# Node Title

[One-sentence summary of what this node documents.]

---

## [Section 1 — primary content]

[Substantive content with inline epistemic labels. Example:]

The gene encodes a protein that performs X [✅ CITATION]. It is expressed predominantly in Y [🔶 CITATION]. Whether it also performs Z is unknown [❓].

---

## [Section 2 — secondary content]

[Continue as needed. Each section should cover one coherent sub-claim or evidence layer.]

---

## Linked nodes

- [[NodeID1]] — [one sentence: why this connection exists]
- [[NodeID2]] — [one sentence: why this connection exists]

---

## Open questions

1. [Specific question directly motivated by evidence gaps in this node]
2. [Another question]
```

**Required YAML fields:** `tags`, `node_type`, `tier`, `epistemic_status`, `last_updated`, `linked_nodes`.

**Optional YAML fields:** `hypothesis_seeds`, `open_questions`. These are included whenever the node's evidence naturally suggests either — which is most of the time.

**`epistemic_status` in the YAML frontmatter** is a node-level summary of the dominant epistemic weight of the node's content. It does not replace claim-level labels in the body text. A node with mostly established claims and one speculative inference should have `epistemic_status: mixed` in the frontmatter and carry the appropriate inline label on the speculative claim.

---

## YAML frontmatter field reference

| Field | Type | Required | Values / Format |
|-------|------|----------|-----------------|
| `tags` | list of strings | Yes | `[gene-wiki, tier1-molecular, ...]` |
| `node_type` | string | Yes | `molecular`, `pathway`, `phenotype`, `disease-connection`, `synthesis`, `contested-claims` |
| `tier` | integer | Yes (node files) | `1`, `2`, `3`, `4` |
| `epistemic_status` | string | Yes | `established`, `emerging`, `speculative`, `unknown`, `mixed` |
| `last_updated` | ISO date | Yes | `YYYY-MM-DD` |
| `linked_nodes` | list of wikilinks | Yes | `["[[NodeID]]", ...]`; empty list `[]` if none |
| `hypothesis_seeds` | list of strings | No | plain language hypothesis statements |
| `open_questions` | list of strings | No | plain language gap statements |
| `version` | string | No | for synthesis files that track major revisions |

---

## Edge mapping protocol

### What is an edge?

An edge is a directed mechanistic or evidential connection between two nodes. "A → B" means: information or material from node A flows into, constrains, or directly enables the content of node B. Edges are not thematic proximity — two nodes about the same gene are not connected by an edge unless one's content causally or evidentially depends on the other's.

### Edge types

**Confirmed edges** are directly evidenced in a cited primary study. The study must explicitly measure or report the connection in question, not merely be consistent with it.

**Inferred edges** are mechanistically motivated but not directly demonstrated. The source node's evidence creates a strong prior for the connection, but the specific connection has not been measured in the relevant system.

### EDGE-MAP.md format

The EDGE-MAP.md file is a flat registry of all edges in the wiki, organized into two sections (confirmed and inferred), each as a Markdown table:

```markdown
## Confirmed edges

| Source node | Target node | Edge description | Epistemic status | Primary citation |
|-------------|-------------|-----------------|-----------------|-----------------|
| [[T1-Protein]] | [[T2-Pathway]] | Protein X transports substrate Y into the TCA cycle | ✅ Established | Author-Year |

## Inferred edges

| Source node | Target node | Edge description | Inference basis | Evidence needed |
|-------------|-------------|-----------------|----------------|----------------|
| [[T2-Pathway]] | [[T4-Disease]] | Pathway dysregulation in node A is proposed to contribute to disease in node B | Mechanistic coherence | Direct measurement in relevant cell type |
```

### edge-map.csv

A machine-readable version of the edge map should be maintained alongside EDGE-MAP.md. Columns: `source`, `target`, `edge_type` (confirmed/inferred), `epistemic_status`, `description`, `citation`. This file is generated manually from EDGE-MAP.md and updated at each wiki version release.

---

## Synthesis files

In addition to the tier node files, every wiki should include six synthesis files at the wiki root. These are not nodes — they do not carry tier labels or `node_type: molecular/pathway/phenotype/disease-connection`. They carry `node_type: synthesis` or `node_type: contested-claims`.

| File | Purpose |
|------|---------|
| `00-INDEX.md` | Master index of all nodes with a Mermaid graph and tier-by-tier node table |
| `EDGE-MAP.md` | Complete edge registry (confirmed + inferred) and top connection gaps |
| `HYPOTHESES.md` | Full hypothesis registry with classification, evidence chain, test design, falsification |
| `RESEARCH-AGENDA.md` | Prioritized study list by time horizon (short / medium / long-term) |
| `MISSING-LINKS.md` | Broken wikilinks, unverified citations, unresolved cross-references |
| `CONTESTED-CLAIMS.md` | Formal register of internal contradictions with resolution evidence |

### When to create synthesis files

Create all six synthesis files after completing the tier node files, not before. The synthesis files depend on the nodes being populated — building them first leads to placeholder content that has to be rewritten.

---

## Hypothesis classification rubric

Every hypothesis in HYPOTHESES.md is classified as Tier A (Conservative), Tier B (Intermediate), or Tier C (Radical) using the following criteria:

### Tier A — Conservative

**Criteria:** The hypothesis follows directly from established or emerging evidence in Tier 1 or Tier 2. If correct, it confirms a mechanistic inference already present in the literature. It does not require overturning any standing assumption. The experiment that would test it is clearly specified and feasible within 18 months using standard methods.

**Prior probability:** High (>50% plausible given current evidence).

**What this tier is for:** Hypotheses that frame the next obvious experiment — important for the field, not speculative, testable now.

---

### Tier B — Intermediate

**Criteria:** The hypothesis connects two or more evidence layers from different tiers in a way that has not been explicitly proposed in the literature, or extends a Tier A hypothesis to a new context (different tissue, developmental stage, species). It may require revisiting an assumption about one node's role, but does not require overturning a well-established finding. The test is designable but may require collaboration or new model systems.

**Prior probability:** Moderate (20–50% plausible given current evidence).

**What this tier is for:** Hypotheses that are worth pursuing but would genuinely surprise some experts in the field if confirmed.

---

### Tier C — Radical

**Criteria:** The hypothesis proposes a connection that would require overturning a standing assumption in the field, or that connects the gene's biology to an adjacent disease or field in a way that is supported by evidence but would be considered extraordinary by most experts. Confirmation would constitute a major finding. The test is demanding and may require methods or models not yet established.

**Prior probability:** Low to moderate (5–30% plausible given current evidence), but the scientific impact of confirmation is proportionally high.

**What this tier is for:** Hypotheses that are too important to leave implicit. Making them explicit with an evidence chain and a falsification criterion is the most valuable contribution of the framework's speculative tier.

---

### Hypothesis entry format

Each hypothesis in HYPOTHESES.md follows this structure:

```markdown
## H[A/B/C][N] — [Short title]

**Classification:** Tier [A / B / C] ([Conservative / Intermediate / Radical])

**Hypothesis statement:** [One or two sentences. Should be specific enough that a test design follows directly from it.]

**Evidence chain:**
- [Evidence layer 1 with epistemic label and citation]
- [Evidence layer 2]
- [Inference step connecting the layers]

**Proposed test:** [The most direct experiment or analysis that would confirm or refute the hypothesis. Should specify: system (cell line / animal / human cohort / public dataset), key measurement, expected result if the hypothesis is correct.]

**Falsification criterion:** [What specific result would refute the hypothesis? A hypothesis with no falsification criterion should not be classified — it is a speculation, not a hypothesis.]

**Linked nodes:** [[NodeID1]], [[NodeID2]]

**Linked edge gap:** [Reference to the EDGE-MAP gap this hypothesis would close, if applicable]
```

---

## Curation workflow

### Adding a new paper

1. Read the paper and identify which nodes it is relevant to (one paper may be relevant to multiple nodes).
2. For each relevant node: open the node file, add the finding as a new sentence or paragraph with an inline epistemic label and citation. Update `last_updated` in the frontmatter.
3. If the paper introduces a finding not covered by any existing node, consider whether a new node is warranted. A new node is warranted if the finding represents a distinct, coherent evidence unit that will be linked to by at least two other nodes. A single finding rarely warrants its own node.
4. If the paper contradicts a claim in an existing node, assess severity: minor correction (update the label and add a caveat sentence), material contradiction (add to CONTESTED-CLAIMS.md and update both affected nodes), or major revision (update the epistemic label and revise the synthesis text).
5. If the paper enables an edge that was previously inferred to be reclassified as confirmed, update EDGE-MAP.md.
6. Update MISSING-LINKS.md if any previously flagged unverified citation has now been confirmed or refuted.

### Epistemic label upgrade procedure

An epistemic label upgrade (Speculative → Emerging, Emerging → Established) is triggered when new evidence crosses a threshold:

- **Speculative → Emerging:** A primary study directly measures the claimed connection in a relevant system and reports a positive result. Label upgrades to Emerging even if the study has limitations (small n, single lab).
- **Emerging → Established:** At least one independent replication using a different method or system confirms the finding, with no credible contrary evidence.

When upgrading a label:
1. Update the inline label in the relevant node file.
2. Update `epistemic_status` in the YAML frontmatter if this was the dominant claim.
3. Update `last_updated`.
4. If the upgraded claim was in CONTESTED-CLAIMS.md as an unresolved contradiction, mark it as resolved with the resolving citation.
5. If any inferred edges in EDGE-MAP.md were blocked on this claim being speculative, assess whether they can now be reclassified as confirmed or upgraded to inferred-with-strong-support.

---

## Version release protocol

The wiki is maintained as a versioned archive. A new version release should be created when:

- A major new finding materially changes the epistemic status of a central claim (e.g., a clinical trial result, a gene therapy approval, a negative replication of a key hypothesis).
- More than 20% of nodes have been updated since the last release.
- A synthesis file has been substantively revised (new hypotheses added, contested claims resolved).

**Release naming:** Semantic versioning. v1.0 = initial public release at manuscript submission. v1.1, v1.2 = minor updates (new papers, label corrections). v2.0 = major revision (new tier, new synthesis files, substantial hypothesis changes).

**Release procedure:**
1. Update `last_updated` in all modified files.
2. Update `00-INDEX.md` if node count or Mermaid graph has changed.
3. Regenerate `edge-map.csv` from EDGE-MAP.md.
4. Create a GitHub release with a brief changelog describing what changed and why.
5. Zenodo automatically archives the release and issues a new DOI (via the GitHub-Zenodo integration).
6. The concept DOI (which always resolves to the latest version) remains stable and does not need to be updated in any citations.

---

## Applicability guidance

This framework is best suited for genes with the following characteristics:

- At least 10–15 published papers providing primary evidence at Tier 1 or Tier 2 (below this, there is insufficient material to populate a meaningful graph).
- A known rare disease connection, providing the clinical anchor for Tier 3.
- Evidence that crosses at least two biological scales (molecular + pathway, or pathway + phenotype), enabling edge mapping.
- At least one area of genuine mechanistic uncertainty or internal contradiction, which is where the framework adds the most value over a narrative review.

The framework is less useful for:

- Genes with fewer than five published papers (too little evidence to populate two tiers meaningfully; a narrative summary is more appropriate).
- Genes where the disease mechanism is largely resolved and the research frontier is therapeutic optimization rather than hypothesis generation.
- Genes with very large evidence bases (hundreds of papers per tier) where the bottleneck is not synthesis but data management — in that case, formal ontologies and database integration are more appropriate tools.

---

## Citation

If you use this framework to build a wiki for a different gene, please cite the reference paper and note the gene and disease in your acknowledgments:

> Freitas HR et al. (2026). A structured epistemic knowledge graph for hypothesis generation in rare disease research: proof of concept in SLC13A5 citrate transporter disorder (DEE25). *Orphanet Journal of Rare Diseases* [DOI to be assigned]. Framework specification v1.0: [ZENODO DOI].

If you extend the framework (new tier definitions, new epistemic label criteria, new synthesis file types), please open a GitHub issue or pull request so that extensions can be reviewed and potentially incorporated into future specification versions.
