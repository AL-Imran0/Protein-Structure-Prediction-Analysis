# 🧬 Protein Structure Prediction & Analysis

## Project Overview
This project demonstrates a **complete pipeline for protein structure prediction and analysis** using synthetic sequences. It integrates sequence preprocessing, feature extraction, structure prediction (via ESMFold or a mock predictor), and structural analysis through RMSD, per-residue deviations, and PCA.  

It provides a **research-ready workflow** for educational purposes, benchmarking, or extension to real protein data.

---

## Features
- **Synthetic sequence generation** with length filtering and uniqueness checks  
- **Sequence feature extraction**:  
  - Length  
  - Hydrophobic fraction  
  - Charged fraction  
  - Amino acid composition  
- **Structure prediction**:  
  - ESMFold (GPU recommended)  
  - Mock alpha-helix generator (fallback)  
- **Experimental PDB simulation** using Gaussian noise and random rotations  
- **Structural analysis**:  
  - RMSD (global and per-residue) using the Kabsch algorithm  
  - PCA visualization of CA coordinates  
- **Visualizations**:  
  - RMSD barplots, histograms, and boxplots  
  - Correlation heatmaps of sequence features vs RMSD  
  - Per-residue RMSD line plots  
  - PCA-based 3D scatter plots  
  - Optional interactive 3D overlays using `py3Dmol`  
- **Research summary table** includes RMSD, per-residue RMSD, and sequence features  

---

## Installation & Requirements

### Python Packages
```bash
pip install biopython py3Dmol scikit-learn matplotlib pandas torch seaborn einops
pip install git+https://github.com/facebookresearch/esm.git
pip install openfold
