---
layout: work
title: Skills and Proficiencies
permalink: /skills
order: 1
intro: The methodology implemented for any NGS project depends on the data modality, the project design, and the hypotheses being tested. Since 2020 I have worked extensively with whole-genome and whole-transcriptome sequencing datasets; each dataset presents unique requirements that necessitates flexible pipeline development. Here, I summarize core methods that highlight the breadth and depth of my NGS analysis toolbox.
items:
  - title: Clustering
    image:
      src: /assets/img/cluster.png
      alt: cluster TSNE
    description: A primary goal of NGS analysis is the identification of biologically meaningful populations (e.g. cell types, spatial domains). Traditionally, this process requires clustering analysis, although the method used depends on certain qualities of the NGS data. For single-cell and single-nuclei RNA-sequencing, k-means clustering and graph-based clustering (Leiden, Louvain) are often successful, but for spatial transcriptomics data I have used methods that leverage the presence of known spatial locations (Banksy, BayesSpace, PRECAST). I have also obtained cluster-free annotations by projecting reduced dimension representations (e.g. PCA, NMF) of reference cell types onto a query dataset. This approach can be particularly useful to standardize annotations across diverse datasets (e.g. multi-model, cross-species). 
  - title: Differential expression models
    image:
      src: /assets/img/volcano.png
      alt: volcano plot
    description: Differential expression (DE) modeling is fundamental to most hypothesis testing with NGS data and I have implemented both single-observation models for RNA-seq (MAST, Wilcoxon signed rank test) and pseudo-bulk observation models for RNA-seq and ATAC-seq (limma, edgeR, DESeq2). I have performed DE modeling for both simple and complex experimental designs, gaining both the experience and statistical expertise to navigate the many assumptions and considerations that make a critical difference when interpreting DE models.
  - title: Gene sets and networks
    image: 
      src: /assets/img/gene-net.png
      alt: gene network
    description: I typically identify genes of interest through DE modeling and gene co-expression networks. I have used both gene set enrichment analysis (fgsea) and over-representation analysis (clusterProfiler, EnrichR) to extract biological information by querying a variety of annotation databases (GO, REACTOME, STRING). With transcriptomic data I have used gene regulatory network analysis (GRNBOOST2, SCENIC) to identify modules of co-expressed disease-associated genes and to find transcription factors that could explain NGS gene sets. With paired RNA-seq and ATAC-seq multiomic data more GRN analyses are possible (SCENIC+, Linger); I have also performed motif enrichment and peak-to-gene linkage analysis (ArchR, Signac).
  - title: Genetic Integration
    image:
      src: /assets/img/dna.png
      alt: DNA helix
    description: Integrating transcriptomic and genomic datasets is a powerful way to probe gene-by-environment interactions that could contribute to disease etiology. In the absence of paired genomic sequencing, I have leveraged GWAS data to estimate the relevance of gene sets to human disease (MAGMA, s-LDSC). With paired genomic data, I have used eQTL and colocalization analysis to identify potential causal variants linked to genetic risk for mood disorders. I am actively expanding by toolset to include mendelian randomization analysis that more directly tests for causal association between genetic variants and gene expression.
---

<p>
  Working with NGS data requires extensive organization and documentation, often implemented in high-performance computing environments and achieved with tools like Github for version control and conda or pip package management. My experience with different sequencing techniques has given me the skills to be comfortable processing NGS data from fastq files, manually performing quality control, barcode extraction, read alignment, and read quantification. Across the years I have used R and Python extensively, executing code with bash scripts, Jupyter Notebook, and integrated development environments like RStudio and PyCharm. I have worked with all of the major NGS processing pipelines including BioConductor, Seurat, and scanpy workflows.
</p>
