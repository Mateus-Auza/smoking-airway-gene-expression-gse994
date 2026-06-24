# Smoking-associated gene expression analysis (GSE994)

## Overview

This project presents a transcriptomic re-analysis of the landmark study:

**Spira et al. (2004)**  
*"Effects of cigarette smoke on the human airway epithelial cell transcriptome"*  
DOI: 10.1073/pnas.0401422101

The objective of this report is to reproduce and extend the original findings by investigating how cigarette smoking alters airway epithelial gene expression, and whether these molecular changes persist after smoking cessation.

The analysis uses the GEO dataset **GSE994**, containing gene expression profiles from:

- Current smokers
- Former smokers
- Never smokers

with a total of **75 patient samples** and **22,215 transcriptomic features**.

---

## Main analyses

### 1. Exploratory Data Analysis

The dataset structure and global transcriptomic variability were investigated using:

- Expression distribution analysis
- Principal Component Analysis (PCA)
- Hierarchical clustering
- Gene variability analysis

These analyses evaluate whether smoking status explains the major sources of transcriptomic variation.

---

### 2. Identification of smoking-associated gene expression changes

Current smokers were compared with never smokers using two complementary approaches:

- Classical Student's t-test with permutation-based significance estimation
- **limma** empirical Bayes differential expression analysis

The resulting gene signatures were evaluated using:

- Hierarchical clustering
- Signature overlap analysis
- Comparison with the original 2004 study

---

### 3. Persistence of smoking-induced alterations

Former smokers were incorporated to investigate whether smoking-associated transcriptional changes remain after cessation.

The analysis identifies genes showing persistent alterations between:

- Former smokers
- Never smokers

and compares results between:

- Historical statistical approaches
- Modern statistical pipelines

---

### 4. Volcano plot analysis

A complementary genome-wide differential expression analysis was performed using limma.

The volcano plot integrates:

- Statistical significance
- Biological effect size (log2 fold change)

to visualize smoking-associated transcriptomic changes across the complete dataset.

---

## Main findings

- Smoking status does not explain the largest global transcriptomic variation, which appears driven by individual biological variability and potential confounding factors.
- Differential expression analysis identifies a robust smoking-associated molecular signature.
- Modern statistical approaches (limma and t-test based methods) recover highly concordant gene sets.
- Several smoking-induced transcriptional changes persist after cessation, suggesting a long-lasting molecular imprint.

---

## Project report

The complete interactive HTML report is available as:

`LSTAT2340.html`

⚠️ **Note:** GitHub cannot display a preview of this HTML file because it exceeds GitHub's file rendering limits.

To view the report:

1. Download the repository ZIP file
2. Extract the files locally
3. Open `report.html` in a web browser

---

## Authors

**Auza Cruz Mateus**  
**Napolitano Dorian**

Published: May 15, 2026

---

## Dataset

Gene Expression Omnibus (GEO):

**GSE994**

Original publication:

Spira et al. (2004)  
*"Effects of cigarette smoke on the human airway epithelial cell transcriptome"*

---

## Tools and methods

Analysis performed using:

- R / Bioconductor
- limma
- Differential expression analysis
- PCA
- Hierarchical clustering
- Transcriptomic visualization methods

---
