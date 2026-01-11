---
layout: work
title: Skills and Proficiencies
permalink: /skills
order: 2
intro: The methodology implemented for any NGS project depends on the data modality, the project design, and the hypotheses being tested. For the past five years I have worked extensively with RNA-sequencing data (single-cell, single-nuclei, spatial, long-read) and multiomic sequencing data (paired single-nuclei RNA-sequencing and ATAC-sequencing). Here, I summarize methods that highlight my expertise with NGS analysis, gathered over many different projects.
items:
  - title: Clustering
    image:
      src: /assets/img/cluster.png
      alt: cluster TSNE
    description: A primary goal of NGS analysis is the identification of biologically meaningful cell populations (e.g. cell types). This process almost always requires clustering analysis, although the method used depends on certain qualities of the NGS data. For single-cell and single-nuclei RNA-sequencing I have success with k-means clustering and graph-based clustering (Leiden, Louvain), depending on the complexity of the dataset. For spatial transcriptomics data, I have used several clustering methods that leverage the presence of known spatial locations (Banksy, BayesSpace, PRECAST). 
  - title: Integration
    image:
      src: /assets/img/dna.png
      alt: DNA helix
    description: There are different motivations for integrating NGS data. Large sequencing studies are often sequenced in batches that introduce un-wanted techinical variation that I have addressed with different tools that each have a unique statistical approach (Seurat, FastMNN, Harmony, scVI). NGS data from different modalities or from different species can be integrated through the subsequent use of label transfer (Seurat, scVI, NMF). A current priority in clinical research is to integrate genomic and transcriptomic sequencing. In the absence of paired genomic sequencing, I have leveraged GWAS data to estimate the relevance of gene sets to human disease (MAGMA, s-LDSC). With paired genomic data, I am currently performing eQTL analysis and mendelian randomization analysis to directly integrate genomic and transcriptomic information.
  - title: Differential expression models
    image:
      src: /assets/img/volcano.png
      alt: volcano plot
    description: Pseudobulk (limma/ edgeR (eBayes), DESeq2 (apeglm shrinkage)), Single-cell (MAST, Wilcoxon), ATAC differential accessibility
  - title: Gene sets and networks
    image: 
      src: /assets/img/gene-net.png
      alt: gene netword
    description: GSEA (fgsea), ORA (clusterProfiler, EnrichR), hdWGCNA, scGREAT, SCENIC
---

<p>
  Working with NGS data requires extensive organization and documentation, often implemented in high-performance computing environments and achieved with tools like Github for version control and conda or pip package management. My experience with different sequencing techniques has given me the skills to be comfortable processing NGS data from fastq files, manually performing quality control, barcode extraction, read alignment, and read quantification. Across the years I have used R and Python extensively, executing code with bash scripts, Jupyter Notebook, and integrated development environments like RStudio and PyCharm. I have worked with all of the major NGS processing pipelines including BioConductor, Seurat, and scanpy workflows.
</p>
