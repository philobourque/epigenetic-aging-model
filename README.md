# epigenetic-aging-model

A computational framework for analyzing CpG methylation data and developing epigenetic aging models.

## 🌟 Purpose

This repository aims to understand how CpG methylation changes across age, tissues, and individuals — and to build predictive models ("epigenetic clocks") ranging from simple linear baselines to deep neural networks. The initial focus is the well-established **GSE40279** blood methylation dataset (656 individuals × ~450k CpGs).

## 🎯 Project Objectives

### 1. Data Infrastructure
- Download and preprocess large Illumina 450K/EPIC methylation datasets
- Align metadata (age, sex, tissue, batch, etc.)
- Efficiently handle high-dimensional CpG matrices

### 2. Biological Exploration
- Study CpG-level methylation distributions
- Identify age-associated CpGs
- Compare methylation signatures across tissues

### 3. Modeling
- Build baseline models (linear regression, ElasticNet)
- Build deep-learning models (MLPs, CNNs, transformers)
- Evaluate cross-tissue generalization
- Compare model stability and feature importance

### 4. Broader Goals
- Identify conserved aging CpGs
- Explore links between CpG drift and known biological aging processes
- Provide reproducible notebooks and scripts

## 📁 Repository Structure

```
epigenetic-aging-model/
│
├── data/
│   ├── raw/              # Untouched downloaded data
│   └── processed/        # Cleaned, filtered, normalized files
│
├── notebooks/
│   └── 01_load_blood.ipynb  # Data exploration & first visualizations
│
├── scripts/
│   ├── load_data.py
│   ├── preprocess.py
│   └── models/
│
├── results/
│   ├── figures/
│   └── model_outputs/
│
└── README.md
```

## 🚧 Project Status: In Progress

- Data loaded successfully
- Exploring CpG distributions and metadata
- Building preprocessing pipeline
- Modeling stage planned next

## 📝 Future Work

- Add automated preprocessing script
- Implement ElasticNet epigenetic clock
- Create cross-tissue benchmarking notebook
