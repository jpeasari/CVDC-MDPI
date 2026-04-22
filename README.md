# 🧬 Phylogenetic Tree & Heatmap Pipeline

This repository contains a custom Python workflow to generate **phylogenetic trees** and **virulence factor heatmaps** from bacterial genomes.

---

## 📌 Overview

- Virulence factors identified using ABRicate with VFDB  
- Heatmaps generated from ABRicate outputs (`ABRicate_Heatmap.ipynb`)  
- Phylogenetic analysis performed using REALPHY and IQ-TREE  
- Custom Python script used for tree formatting and visualization  

---

## 🧪 Data

- 28 genomes (Pasteurellaceae, *Spirabiliibacterium*, CVDC isolates, *S. mucosae* TN_CUL_2021)  
- Reference genomes from NCBI  

---

## ⚙️ Workflow

1. Run ABRicate on genomes  
2. Generate heatmap (`abricate.ipynb`)  
3. Align sequences with REALPHY  
4. Build tree with IQ-TREE (`.tree` file)  
5. Run Python script:
   - Input: `.tree`  
   - Output: `formatted_tree.nwk` + final tree  

---

## ▶️ Usage

```bash
# Heatmap
jupyter notebook abricate.ipynb

# Phylogenetic tree
python tree_script.py --input your_tree.tree
