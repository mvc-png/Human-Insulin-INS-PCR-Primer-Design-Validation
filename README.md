# Human-Insulin-INS-PCR-Primer-Design-Validation
A Python-based project focused on designing highly specific PCR primers for the human insulin (INS) mRNA transcript. This repository includes the structural design strategy, primer metrics, and a Python validation script to calculate GC content.

# Project Overview
The goal is to design an optimized pair of primers to amplify human insulin cDNA via PCR/qPCR while avoiding genomic DNA contamination.
Target Template: Homo sapiens insulin (INS), mRNA (NCBI Reference Sequence: `NM_000207.3`)
Template Length: 465 bp

# Selected Primer Pair
Forward Primer (5'->3'): `TCAGAAGAGGCCATCAAGCA` (Starts: 22, Stop: 41)
Reverse Primer (5'->3'): `CCCGCACACTAGGTAGAGAG` (Starts: 191, Stop: 172)
Expected PCR Product Length: 170 bp

# Thermodynamic Properties
| Primer | Length | Melting Temp (Tm) | GC % | Self-Complementarity |
| Forward | 20 bp | 59.01°C | 50.0% | 4.00 |
| Reverse | 20 bp | 58.97°C | 60.0% | 4.00 |
A Tm difference of 0.04°C, aids in synchronized annealing.

# Design Strategy & Results
To ensure high specificity and prevent the amplification of contaminating genomic DNA, the Forward Primer was designed to span an exon-exon junction (located at boundary 41-42). 
Since the forward primer spans an exon junction, it will only bind to fully processed mRNA/cDNA and not amplify genomic DNA contamination making the assay cleaner.
