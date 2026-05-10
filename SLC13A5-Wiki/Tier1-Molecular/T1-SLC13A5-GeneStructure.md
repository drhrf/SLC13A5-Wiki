---
tags: [slc13a5-wiki, tier-1, molecular, gene-structure, genomics]
tier: 1
node_type: molecular
epistemic_status: established
last_updated: 2026-05-10
linked_nodes:
  - "[[T1-SLC13A5-Protein]]"
  - "[[T1-VariantCatalog]]"
  - "[[T1-ExpressionAtlas]]"
  - "[[T1-INDYOrthologs]]"
  - "[[T2-TranscriptionalRegulation]]"
hypothesis_seeds:
  - "Brain-specific regulatory elements may be distinct from liver elements and could be targeted to restore SLC13A5 selectively in neurons"
  - "Noncoding variant burden in regulatory elements could explain phenotypic variability not explained by coding variants"
open_questions:
  - "What noncoding regulatory elements (enhancers, silencers) control SLC13A5 expression in human cortical neurons specifically?"
  - "Are there brain-specific transcript variants with distinct regulatory or protein-isoform properties?"
  - "Does the gene harbor common regulatory variants that modify expression level in brain and contribute to dementia risk?"
---

# SLC13A5 Gene Structure

## Core claim

SLC13A5 (solute carrier family 13, member 5) is located on human chromosome 17p13.1 and encodes NaCT, a sodium-coupled citrate transporter. The gene was identified as the cause of neonatal epileptic encephalopathy (EIEE25/DEE25) through exome sequencing of multiplex families in 2014. It is also known as mINDY, the mammalian ortholog of the *Drosophila* longevity gene *I'm Not Dead Yet*. Source: [[genes/SLC13A5]], [[research/Thevenon-2014]].

## Mechanism

The genomic organization of SLC13A5 consists of multiple exons encoding an 11-transmembrane domain protein (NaCT). The gene uses a sodium-dependent cotransport mechanism, coupling the import of one citrate trianion (citrate³⁻) to three sodium cations (Na⁺) in an electrogenic process. The protein architecture is dictated by the gene's exon structure, with the transport domain and scaffold domain encoded by distinct exonic regions — a feature shared across the SLC13 family.

Transcriptional regulation differs dramatically between tissues. In liver, PXR (pregnane X receptor) and AhR (aryl hydrocarbon receptor) drive SLC13A5 expression through xenobiotic-response elements in the promoter region. In brain, the co-expression network analysis by [[research/Ferreira-2026]] shows the SLC13A5 co-expression module enriched for NFE2/NRF-like, TFAM-associated, and AP-1 family transcription factor binding motifs — consistent with mitochondrial biogenesis regulatory logic rather than xenobiotic response.

The human gene has a paralogous relationship with SLC13A3 (NaDC3) and SLC13A2 (NaDC1), both sodium-dicarboxylate transporters, but SLC13A5 is distinct in its substrate preference for citrate over dicarboxylates and in its tissue distribution pattern. Selectivity over NaDC1/NaDC3 is conferred by four scaffold domain residues (Leu56, Ala57, Gly409, Ile410) identified in the cryo-EM structure ([[research/Sauer-2021]]).

## Evidence basis

- Source 1: [[genes/SLC13A5]] — comprehensive gene/protein overview including regulatory elements, expression, variant map, and species differences.
- Source 2: [[research/Thevenon-2014]] — gene discovery paper; biallelic mutations in sodium-binding residues as cause of neonatal epileptic encephalopathy.
- Source 3: [[research/Sauer-2021]] — cryo-EM structure defining domain architecture, sodium-binding sites, substrate pocket, and selectivity determinants.
- Source 4: [[research/Ferreira-2026]] — WGCNA defining brain-side transcription factor enrichment (NFE2/NRF/TFAM motifs) in the SLC13A5 co-expression module.
- Source 5: [[mechanisms/SLC13A5-transcriptional-regulation]] — comprehensive review of PXR, AhR, CAR-independent phenobarbital induction, and brain regulatory uncertainty.

## Connections to other nodes

- Feeds into [[T1-SLC13A5-Protein]] — gene encodes the NaCT protein whose structure and function are the downstream subject.
- Upstream of [[T1-VariantCatalog]] — gene structure determines which residues tolerate substitution (DMS data) and which variant classes arise.
- Regulated by [[T2-TranscriptionalRegulation]] — the regulatory elements in the gene promoter/enhancers govern tissue-specific expression.
- Contextualizes [[T1-ExpressionAtlas]] — genomic location and regulatory logic determines the tissue and cell-type expression patterns.
- Evolutionary context in [[T1-INDYOrthologs]] — the *Drosophila* INDY, C. elegans *indy-1*, and mouse *Slc13a5* orthologs share the core gene structure but differ in transport capacity and regulation.

## Open questions

1. Which specific enhancer elements drive SLC13A5 expression in cortical neurons during the first postnatal year, when [[research/Ferreira-2026]] shows peak cerebrum expression — and are these elements accessible by AAV-delivered transcription factor overexpression?
2. Does SLC13A5 produce alternative transcripts in brain that encode protein isoforms with different Km values or regulatory behavior, distinct from the hepatic form?
3. Are common regulatory variants in the SLC13A5 locus (eQTLs in GTEx brain data) associated with plasma citrate levels in UK Biobank, and do those variants predict cognitive performance as tested by [[queries/hypotheses-SLC13A5-dementia-Alzheimer]]?
4. Does the SLC13A5 promoter contain CpG islands whose methylation changes with age in human brain — providing a mechanism for the declining cerebrum expression trajectory observed by [[research/Ferreira-2026]]?
