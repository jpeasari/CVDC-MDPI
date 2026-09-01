# 🧬 Phylogenetic Tree & Heatmap Pipeline

This repository provides a custom Python workflow for visualizing phylogenetic trees and generating heatmaps of virulence factors derived from bacterial genomes.

---

## 📌 Overview

- Virulence factors identified using ABRicate with VFDB  
- Heatmaps generated from ABRicate outputs (`Create_Abricate_Heatmap.ipynb`)  
- Phylogenetic analysis performed using REALPHY and IQ-TREE  
- Custom Python script used for tree formatting and visualization  

---

## 🧪 Data

- 28 genomes (Pasteurellaceae Genomes) 
- 25 genomes were downloaded from NCBI, Spirabiliibacterium mucosae TN_CUL_2021 provided by the original author and 2 CVDC Isolates 

---


## ⚙️ Workflow Phylogenetics Tree
   
1. Align sequences with REALPHY  
2. Build tree with IQ-TREE (`.tree` file)  
3. Run Python script:
   - Input: `polymorphisms_move.phy.treefile`  
   - Output: `formatted_tree.nwk` + `JVDI_Figure1.tif`

## ⚙️ Workflow ABRicate Heatmap

1. Run ABRicate on genomes  
2. Generate heatmap using `ABRicate_Heatmap.ipynb`
   - Input: `abricate_all_updated.csv`
   - Output: `JVDI_Figure2.tif`

---


