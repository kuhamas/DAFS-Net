# DAFS-Net
DAFS‑Net integrates genomic (SNPs), transcriptomic, and  methylation data to predict complex plant traits (e.g., flowering time, yield). It uses adaptive feature scaling, learnable sparse graph attention (HardConcrete gates + joint sparsity), and multi‑view attention fusion. Provides global feature importance and per‑sample omics contributions. Outperforms single‑omics and state‑of‑the‑art multi‑omics methods on Arabidopsis, maize, and rice.
# DAFS‑Net – Multi‑Omics Genomic Prediction

This repository contains the complete code, data, and supplementary materials for the **DAFS‑Net** (Differentiable Adaptive Feature Scaling and Graph Network) model, as described in our paper:

> *DAFS‑Net: Differentiable Adaptive Feature Scaling and Graph Network for Multi‑Omics Trait Prediction*



## Repository Contents
| File / Folder | Description |
|---------------|-------------|
| `DAFS-Net_Model.zip` | Core implementation of DAFS‑Net (AFSC, LSGA, HardConcrete sparsification, dynamic GAT, multi‑view attention). Contains the split Python scripts: `config_data.py`, `models.py`, `train_eval.py`, `main.py`. |
| `Other_DL_Model.zip` | Implementations of deep learning baselines used for comparison in the paper. |
| `Other_ML_Model.zip` | Classical machine learning baselines: Random Forest and Support Vector Machine (SVM). |
| `Arabidopsis_Dataset.zip` | Processed multi‑omics data for *Arabidopsis thaliana* (383 accessions): genomic SNPs, transcriptomic expression, gene‑body methylation, and six phenotype traits (FLT, CLN, RLN, RBN, DoR, SL). |
| `data_Rice210.zip` | Processed Rice210 dataset (210 recombinant inbred lines): genomic bins, transcriptomics, metabolomics, and three agronomic traits (GN, TP, YD). |
| `supplementary_data.zip` | Additional supplementary data from the paper: lists of important genes, flowering‑time gene overlaps, clustering assignments, feature importance tables, etc. |
| `README.md` | This file. |

# Core dependencies for DAFS‑Net
torch>=1.12.0
numpy>=1.21.0
pandas>=1.3.0
scikit-learn>=1.0.0
scipy>=1.7.0
openpyxl>=3.0.0

# Optional but recommended for visualisation (if you want to reproduce figures)
matplotlib>=3.5.0
seaborn>=0.11.0

# Optional for advanced interpretability (Integrated Gradients)
# captum>=0.6.0
## Installation


git clone https://github.com/kuhamas/DAFS-Net.git
cd DAFS-Net
DOI: 10.5281/zenodo.20676147
