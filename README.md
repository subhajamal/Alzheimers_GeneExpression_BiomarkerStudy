# Alzheimers_GeneExpression_BiomarkerStudy


focusing on the analysis of gene expression data in Alzheimer’s disease (AD). The goal of the project was to identify differentially expressed genes (DEGs), perform enrichment analysis, and explore potential biomarkers or drug targets.

---

## 🧠 Project Context

Using human brain tissue samples, we compared gene expression patterns between:
- **Moderate AD patients**
- **Control (normal) subjects**

All code was written in **R**, and the analysis follows a structured biomedical research pipeline.

---

## 📊 Project Steps

### 🔹 Step 1: Data Import
- Clinical metadata: `Blalock_clin_final.csv`
- Gene expression data: `GSE62232_Blalock_geneexp_final.tsv`

### 🔹 Step 2: Data Cleaning & Filtering
- Selected "Moderate" and "Control" subject groups from clinical data
- Filtered expression matrix accordingly

### 🔹 Step 3: Group Identification
- Labeled comparison and baseline groups based on disease status

### 🔹 Step 4: Sanity Check
- Ensured alignment between clinical and expression datasets
- Exported gene features for reference

### 🔹 Step 5: T-Test Preparation
- Checked numeric structure of expression data
- Cleaned input for analysis

### 🔹 Step 6: T-Test Execution
- Used a custom R function to compare gene expression between groups
- Exported full t-test results

### 🔹 Step 7: DEGs Filtering & Enrichment Analysis
- Shortlisted genes with **p-value ≤ 0.05**
- Cleaned gene names and removed duplicates/NA
- Performed enrichment analysis using **Enrichr R package**
- Identified biological pathways and GO categories

---

## 🔄 Cross-Team Comparison

A collaborative Venn diagram analysis was conducted across groups analyzing different AD stages (Early, Moderate, Severe). This highlighted:
- Shared DEGs between groups
- Unique and overlapping pathways
- Candidate genes for AD progression

---

## 📁 Repository Contents
Midterm_GeneExpression_Analysis/ ├── results/ │ ├── Subha_Moderate_Control_TTest.csv │ ├── Subha_Moderate_Control_DEGs.csv │ ├── Subha_Moderate_Control_EnrichR.xlsx │ ├── Subha_Moderate_Control_ShortListedPathways.txt │ └── Subha_Moderate_Control_ShortListedGenes.txt │ ├── scripts/ │ ├── Subha_GroupCompAnalysis.Rmd │ └── Subha_EnrichAnalysis.Rmd │ ├── reports/ │ ├── Subha_GroupCompAnalysis.html │ └── Subha_EnrichAnalysis.html │ ├── summary/ │ └── Subha_MidtermSummary.docx │ ├── README.md └── .gitignore


---

## 🧪 Tools Used

- R / RStudio
- tidyverse
- Enrichr (via enrichR package)
- Venn diagram tools
- Excel (for quick curation and visualization)

---

## 📚 Summary

This analysis contributes to the ongoing research on Alzheimer’s disease by identifying key gene expression signatures and pathways associated with disease progression. The workflow captures core steps in transcriptomics analysis and reflects real-world biomedical research practices.




