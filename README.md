# RPE-Melanocytes

This repository contains Jupyter notebooks for single-cell RNA sequencing (scRNA-seq) data analysis

Notebooks Overview
Notebook 1_a: RPE Control scRNA-seq Analysis

    Description: This notebook reanalyzes scRNA-seq data from GEO (sample GSM5560840), representing Retinal Pigment Epithelial (RPE) control cells.
    Key Analysis:
        Initial quality control, normalization, and clustering using Seurat.
        Principal component analysis (PCA), nearest-neighbor graph construction, clustering using the Leiden algorithm, and UMAP visualization.
        Doublet detection and removal using DoubletFinder.
        Identification of major cell types, including Melanocytes, RPE cells, Pericytes, Macrophages, NK cells, and more.

Notebook 1_b: RPE and Melanocyte Subclustering

    Description: Focuses on further subclustering of RPE and Melanocyte populations from Notebook 1_a.
    Key Analysis:
        Subclustering with a low-resolution setting using PCA and UMAP.
        Identification of marker genes for subclusters, followed by protein-protein interaction (PPI) analysis using STRING and Gene Ontology (GO) enrichment analysis.

Notebook 2: Comparative Analysis of RPE and Melanocyte Clusters

    Description: Performs a comparative analysis of the RPE and Melanocyte clusters, identifying genes uniquely expressed in these populations.
    Key Analysis:
        Merging RPE and Melano clusters for differential expression analysis using FindAllMarkers.
        Heatmap visualization of highly variable genes and enrichment analysis of key molecular pathways through GO and STRING.

Notebook 3_a: Transcription Factor Analysis

    Description: Analyzes transcription factors in the dataset using a curated list from the Animal Transcription Factor Database (AnimalTFDB).
    Key Analysis:
        PCA and re-clustering to investigate transcription factors within RPE and other cell types.
        Hierarchical clustering and cladistics analysis using Cassiopeia and visualization via Interactive Tree of Life (iTOL).

Notebook 3_b: Further Transcription Factor Clustering

    Description: Extends the transcription factor analysis by refining clustering and investigating lineage relationships.
    Key Analysis:
        Re-clustering and further analysis using known marker genes for lineage reconstruction and transcriptional networks.

Notebook 3_c: Additional Marker Gene Analysis

    Description: Provides additional analysis for identifying key marker genes across cell populations.
    Key Analysis:
        Investigating significant genes in each cluster to deepen the understanding of cell-type-specific transcriptional activity.

Notebook 3_d: Gene Regulatory Network (GRN) Inference in RPE Cells

    Description: Applies the SCENIC pipeline for gene regulatory network inference in RPE cells.
    Key Analysis:
        GRN inference using GRNBoost2, regulon definition via cisTarget, and AUCell for transcription factor activity scoring.
        Visualization of regulon activity across RPE and Melano populations.

Notebook 3_e: Further GRN Refinement

    Description: Continues the GRN analysis with refinements and additional regulatory insights.
    Key Analysis:
        Integration of SCENIC results into AnnData, providing further insights into transcriptional programs across cell populations.

Notebook 4_a: Developmental Stage Analysis of RPE Cells

    Description: Analyzes developmental stages (Weeks 4-8) of RPE cells using scRNA-seq data (GSE155121) in Scanpy.
    Key Analysis:
        Quality control and merging of scRNA-seq data across weeks.
        PCA, UMAP, and Leiden clustering, followed by subclustering of RPE populations.

Notebook 4_c: Reanalysis of RPE and Melanocyte scRNA-seq Data

    Description: Reanalyzes scRNA-seq data from GEO (GSE210543), focusing on RPE and Melanocyte subclusters.
    Key Analysis:
        Subclustering based on marker gene expression, re-identification of highly variable genes, and recalculated PCA and UMAP visualization.

Notebook 4_d(1), (2): Stereo-seq Data Analysis for RPE Developmental Stages

    Description: Reanalyzes Stereo-seq data from CNGB (CNP0001543) focusing on developmental stages E14.5 and E16.5.
    Key Analysis:
        PCA and UMAP visualization for spatial analysis of melanocytes and RPE cells within developmental tissue contexts.
        Spatial analysis using Squidpy to explore cellular community organization.

Notebook 5_a: Transcriptomics of Ciona intestinalis Tailbud Development

    Description: Analyzes scRNA-seq data from Ciona intestinalis across various developmental stages (GSE131155).
    Key Analysis:
        Quality control, PCA, and clustering of developmental stages.
        Identification of RPE-related genes, cross-species comparisons with mouse orthologs, and gene regulatory network analysis using STRING.

Notebook 5_b: Ortholog Analysis in Ciona and Mouse

    Description: Extends analysis of Ciona orthologs in mouse models.
    Key Analysis:
        Gene ortholog identification, protein-protein interactions, and biological pathway enrichment for comparative transcriptomics.

Notebook 5_c: Cladistics Tree Construction

    Description: Constructs a parsimony-based cladistics tree using the Cassiopeia toolkit.
    Key Analysis:
        Preparation of dataframes and lineage reconstruction analysis across Ciona genes.

Notebook 6: Phylostratigraphy Analysis of Mouse Genes

    Description: Conducts phylostratigraphy analysis to assign evolutionary origins to genes within the mouse genome.
    Key Analysis:
        Gene mapping to phylogenetic transitions, identification of melanocyte and RPE marker genes, and differential gene expression analysis in Seurat.

Supplementary 3: Single-Nucleus RNA Sequencing of Monkey Pineal Gland and Pigmentary Epithelium from (https://db.cngb.org/nhpca/)

    Description: Analyzes snRNA-seq data from the monkey pineal gland and pigmentary epithelium using Seurat.
    Key Analysis:
        Clustering of nuclei, UMAP visualization, and identification of key cell types including pinealocytes, melanocytes, and RPE cells.
