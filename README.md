# RNA-Seq Differential Expression Analysis using DESeq2

This project demonstrates a complete RNA-seq gene expression analysis workflow using the **DESeq2** package in R.
The goal is to identify **differentially expressed genes** between pregnancy and lactation samples.

Dataset used: **GSE60450 – Mouse Mammary Gland RNA-seq** (downloaded from NCBI GEO).

---

## Project Overview

RNA-seq allows researchers to measure gene expression across different biological conditions.
In this project, we:

1. Download RNA-seq count data from GEO
2. Prepare count matrix and metadata
3. Perform differential expression analysis with DESeq2
4. Visualize results using PCA, Volcano plot, and Heatmap

---

## Project Structure

rnaseq_project
│
├── data/
│   └── GSE60450_counts.txt
│
├── results/
│   ├── deseq2_results.csv
│   ├── PCA_plot.pdf
│   ├── volcano_plot.pdf
│   └── heatmap_top_genes.pdf
│
├── scripts/
│   └── rna_seq_full_pipeline.R
│
└── README.md

---

## Tools and Technologies

* R
* DESeq2
* Bioconductor
* RNA-seq data from NCBI GEO

---

## Analysis Workflow

### 1. Data Download

RNA-seq count data is downloaded from GEO and extracted.

### 2. Data Preparation

* Load gene count matrix
* Create sample metadata
* Define experimental conditions

### 3. Differential Expression

DESeq2 is used to:

* Normalize counts
* Estimate dispersion
* Identify differentially expressed genes

### 4. Visualization

**PCA Plot**
Shows clustering of samples based on gene expression.

**Volcano Plot**
Displays statistically significant genes with large expression changes.

**Heatmap**
Shows expression patterns of the top differentially expressed genes.

---

## Example Output

The pipeline generates:

* PCA plot showing separation of pregnancy and lactation samples
* Volcano plot highlighting significant genes
* Heatmap of top differentially expressed genes
* CSV file containing DESeq2 statistical results

---

## How to Run the Analysis

Clone the repository and run the pipeline:

```bash
git clone https://github.com/your-username/rna-seq-differential-expression-analysis.git
cd rna-seq-differential-expression-analysis
Rscript scripts/rna_seq_full_pipeline.R
```

---

## Author

Sudharshini Kannan
Bioinformatics Learner | RNA-seq | NGS Data Analysis
