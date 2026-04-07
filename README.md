# 🧬 Spatial Transcriptomics Analysis Pipeline

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Scanpy](https://img.shields.io/badge/Bioinformatics-Scanpy-green)](https://scanpy.readthedocs.io/)
[![Squidpy](https://img.shields.io/badge/Spatial_Analysis-Squidpy-orange)](https://squidpy.readthedocs.io/)
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](LICENSE)

## Base study
- Mouse Brain Analysis: Histological structure and genetic implementation cluster similarity analysis with Mouse Brain dataset from 10x Genomics
<img width="1468" height="590" alt="image" src="https://github.com/user-attachments/assets/3f37b4ba-95c5-4bb6-b320-43f500b1d9e6" />

- Tumor Microenvironment: genetic implementation difference analysis of tumor microenvironment with public cancer tissue ST data
<img width="1475" height="590" alt="image" src="https://github.com/user-attachments/assets/3001fe37-f36f-4307-9e5f-3bde51bd1154" />


## 📌 Introduction
This project aims to explore and analyze **Spatial Transcriptomics (ST)** data to uncover the spatial organization of gene expression within tissues. Leveraging the power of **Scanpy** and **Squidpy**, this repository contains an end-to-end pipeline for processing, clustering, and identifying spatially variable genes (SVGs) from 10x Genomics Visium datasets.

The goal is to bridge the gap between histology (morphology) and transcriptomics (gene expression) to understand tissue architecture at a molecular level.

## 🎯 Key Objectives
- **Preprocessing:** Quality control (QC) and normalization of spatial gene expression data.
- **Dimensionality Reduction:** Utilizing PCA and UMAP to visualize high-dimensional transcriptomic landscapes.
- **Spatial Clustering:** Identifying distinct tissue regions (spatial domains) using graph-based clustering (Leiden/Louvain).
- **Spatially Variable Genes (SVGs):** Detecting genes with distinct spatial patterns using Moran’s I statistic or spatial autocorrelation.
- **Visualization:** Integrating histology images with gene expression overlays.

## 📂 Dataset
* **Source:** [e.g., 10x Genomics Visium Public Dataset - Adult Mouse Brain]
* **Description:** This analysis uses the [Dataset Name] which contains [Number] spots and [Number] genes.
* **Note:** The raw data is not included in this repo due to size constraints. Please refer to `data/download_script.sh` to fetch the dataset.

## 🛠 Tech Stack & Methodology
This project demonstrates proficiency in **Bioinformatics** and **Data Science**:

* **Language:** Python
* **Core Libraries:**
    * `Scanpy`: Single-cell analysis framework.
    * `Squidpy`: Spatial omics analysis and visualization.
    * `Anndata`: Annotated data storage.
    * `Matplotlib` / `Seaborn`: Advanced visualization.
    * `Scikit-learn`: Machine learning utilities.

### Analysis Workflow
Please read [project workflow](./project-workflow.md)

## 📊 Sample Results

| UMAP Projection | Spatial Clustering |
|:---:|:---:|
| ![UMAP](./clinical_validation/assets/tme_umap.png) | ![Spatial](./clinical_validation/assets/tme_cluster.png) |
| *Sequence clustering based on gene expression* | *Clusters mapped onto tissue image* |

> **Insight:** 

## 🚀 How to Run
```bash
# Clone the repository
git clone [https://github.com/sn0wsally/self-study-Spatial-Transcriptomics.git](https://github.com/sn0wsally/self-study-Spatial-Transcriptomics.git)

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter Notebook
jupyter notebook notebooks/
