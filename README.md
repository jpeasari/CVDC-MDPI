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

- 28 genomes (Pasteurellaceae Genomes) 
- 25 genomes were downloaded from NCBI, Spirabiliibacterium mucosae TN_CUL_2021 provided by the original author and 2 CVDC Isolates 

---

## ⚙️ Workflow Heatmap

1. Run ABRicate on genomes  
2. Generate heatmap (`ABRicate_Heatmap.ipynb`)

## ⚙️ Workflow Phylogenetics Tree
   
1. Align sequences with REALPHY  
2. Build tree with IQ-TREE (`.tree` file)  
3. Run Python script:
   - Input: `polymorphisms_move.phy.treefile`  
   - Output: `formatted_tree.nwk` + final tree  in tif format

---

## ▶️ Usage

```bash
# Heatmap
jupyter notebook abricate.ipynb

# Phylogenetic tree
python tree_script.py --input your_tree.tree
