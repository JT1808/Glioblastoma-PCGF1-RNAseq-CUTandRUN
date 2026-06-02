# Glioblastoma-PCGF1-RNAseq-CUTandRUN
Integrative RNA-seq and CUT&amp;RUN analysis of PCGF1-mediated epigenetic regulation of GD2 expression in glioblastoma, combining differential gene expression, histone modification profiling, peak annotation, motif discovery, and pathway enrichment analysis.

# Investigating Epigenetic Regulation of GD2 Expression in Glioblastoma

## Overview

Glioblastoma (GBM) is an aggressive and highly lethal brain tumor characterized by rapid growth, extensive invasion, and resistance to conventional therapies. Despite recent advances in immunotherapy, including GD2-targeted Chimeric Antigen Receptor T-cell (CAR-T) therapy, clinical responses in GBM remain limited. A major challenge is the incomplete understanding of the molecular and epigenetic mechanisms regulating GD2 expression in tumor cells.

This project investigates the role of Polycomb Group Factor 1 (PCGF1), a component of the non-canonical Polycomb Repressive Complex 1 (ncPRC1), in regulating GD2 expression in glioblastoma. Previous findings from the Ayad Laboratory identified PCGF1 as a potential regulator of GD2 expression, suggesting that epigenetic modifications may influence the effectiveness of GD2-targeted therapies.

To explore this mechanism, an integrative multi-omics approach was employed using RNA sequencing and CUT&RUN sequencing data generated from wild-type and PCGF1 knockdown LN229 glioblastoma cells. The objective was to characterize transcriptional and epigenetic changes associated with PCGF1 depletion and identify pathways involved in GD2 biosynthesis and glycosphingolipid metabolism.

---

## Research Objectives

- Investigate the role of PCGF1 in regulating GD2 expression in glioblastoma cells.
- Identify transcriptional changes following PCGF1 knockdown using RNA-seq.
- Characterize alterations in chromatin-associated histone modifications using CUT&RUN.
- Identify differential genomic binding regions and consensus peaks between experimental conditions.
- Integrate transcriptomic and epigenomic datasets to uncover pathways associated with GD2 regulation.
- Explore potential epigenetic mechanisms that could enhance GD2-targeted immunotherapies.

---

## Experimental Design

### Cell Model

- LN229 Glioblastoma Cell Line
- Wild-Type (Control)
- PCGF1 Knockdown (PCGF1KD)

### Histone Marks Profiled

CUT&RUN sequencing was performed to evaluate changes in chromatin state and Polycomb-mediated gene regulation using:

- H3K4me3 (active promoter mark)
- H3K27me3 (transcriptional repression mark)
- H2AK119ub1 (PRC1-associated ubiquitination mark)
- IgG control

---

## Bioinformatics Workflow

### RNA-seq Analysis

1. Raw sequencing quality assessment
2. Alignment using STAR
3. Gene-level count generation
4. Differential expression analysis using DESeq2
5. Principal Component Analysis (PCA)
6. Volcano plot and heatmap generation
7. Gene set enrichment analysis using MSigDB

### CUT&RUN Analysis

1. Read alignment using Bowtie2
2. Peak calling using MACS2 and SEACR
3. Consensus peak generation across replicates
4. Peak subtraction and differential peak identification using BEDTools
5. Peak annotation using ChIPseeker
6. Motif discovery using MEME Suite
7. Pathway enrichment analysis using Reactome and MSigDB

---

## Tools and Software

### Sequencing Analysis
- STAR
- Bowtie2
- MACS2
- SEACR
- BEDTools

### Statistical Analysis
- R
- DESeq2
- ChIPseeker
- clusterProfiler
- ReactomePA

### Visualization
- ggplot2
- pheatmap
- ComplexHeatmap

### Motif Analysis
- MEME Suite

---

## Key Findings

### Transcriptomic Changes

PCGF1 knockdown produced distinct transcriptional profiles compared to wild-type glioblastoma cells. Principal component analysis and clustering demonstrated clear separation between experimental groups, indicating reproducible transcriptional alterations following PCGF1 depletion.

Several genes involved in GD2 biosynthesis were significantly upregulated, including:

- ST8SIA1 (GD3 Synthase)
- B4GALNT1 (GD2 Synthase)

These findings suggest that PCGF1 functions as a transcriptional suppressor of pathways involved in GD2 production.

### Epigenetic Alterations

CUT&RUN profiling revealed changes in Polycomb-associated histone modifications following PCGF1 knockdown.

Key observations included:

- Altered H2AK119ub1 occupancy across multiple genomic loci.
- Redistribution of H3K27me3-associated repressive chromatin regions.
- Changes in active promoter-associated H3K4me3 signals.
- Differential peak enrichment in genes associated with glycosphingolipid metabolism.

### Pathway Enrichment

Integrated RNA-seq and CUT&RUN analyses identified enrichment of pathways involved in:

- Glycosphingolipid metabolism
- Glycosphingolipid catabolism
- Cell signaling pathways
- Cellular recognition and membrane-associated processes

These pathways are closely linked to GD2 synthesis and regulation, supporting a mechanistic relationship between PCGF1 activity and GD2 expression.

---

## Biological Significance

The results support a model in which PCGF1 contributes to transcriptional repression through PRC1-mediated chromatin regulation. Loss of PCGF1 disrupts repressive histone modifications, leading to activation of genes involved in GD2 biosynthesis and glycosphingolipid metabolism.

Given the growing interest in GD2-targeted CAR-T therapies for glioblastoma, understanding the epigenetic mechanisms controlling GD2 expression may provide opportunities to enhance therapeutic efficacy through combination approaches targeting chromatin regulators.

---

## Skills Demonstrated

- RNA-seq Analysis
- CUT&RUN Analysis
- Differential Gene Expression
- Peak Calling and Annotation
- Epigenomics
- Cancer Genomics
- Chromatin Biology
- Histone Modification Analysis
- Pathway Enrichment Analysis
- Multi-omics Data Integration
- R Programming
- Linux/Bash
- Data Visualization
- Statistical Genomics

---

## Author

Jhalak Trivedi  
M.S. Bioinformatics, Georgetown University

Research conducted at the Ayad Laboratory, Georgetown Lombardi Comprehensive Cancer Center, under the mentorship of Dr. Rob Suter.
