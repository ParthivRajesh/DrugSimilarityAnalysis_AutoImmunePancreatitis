# Drug Similarity Analysis for Autoimmune Pancreatitis

## Project Overview
This repository contains the workflow and results of a study to identify drugs structurally similar to prednisone for the treatment of Autoimmune Pancreatitis (AIP). AIP is a rare inflammatory condition that responds well to corticosteroid therapy. The goal of this project is to explore potential drug alternatives using computational tools like KNIME.

## Problem Statement
Prednisone, a synthetic corticosteroid, is commonly prescribed for managing AIP. Identifying structurally similar drugs can offer alternative therapeutic options and contribute to drug discovery efforts. This study employs 2D and 3D conformer analyses for this purpose.

## Workflow and Tools
- **Data Source**: PubChem database.
- **Tools Used**: KNIME for computational analysis, leveraging nodes for feature extraction, similarity scoring, and visualization.
- **Analysis Methods**:
  - **2D Similarity**: Tanimoto Coefficients.
  - **3D Alignment**: Root Mean Square Deviation (RMSD).

### Key Steps:
1. **Data Pre-processing**:
   - Molecule retrieval from PubChem.
   - Conversion to standard formats (e.g., SMILES, SDF).
   - Structural normalization.
2. **Feature Extraction**:
   - Calculation of 2D and 3D molecular descriptors.
3. **Similarity Analysis**:
   - Scoring based on Tanimoto (2D) and RMSD (3D).
4. **Visualization**:
   - Scatter plots and heatmaps for interpretability.
5. **Filtering**:
   - Shortlisting compounds with high similarity scores (e.g., Tanimoto > 0.8).

## Results
### Top Similar Drugs:
- **2D Similarity**:
  - Tanimoto Scores: 0.85, 0.90, 0.95, 1.00.
- **3D Similarity**:
  - RMSD Scores: 0.00, 0.25, 0.50, 0.75.

## Conclusion
This project demonstrates the power of computational tools in identifying structurally similar drugs. By combining 2D fingerprint analysis with 3D spatial alignment, a well-rounded approach to molecular similarity evaluation was achieved. The findings provide insights into potential prednisone alternatives for AIP and pave the way for further research in drug discovery.

## Repository Contents
- `workflow/ and visualisation/`: KNIME workflows for 2D and 3D analyses and scatter plots, heatmaps, including other graphical results
- `data/`: Processed and raw datasets used in the study.
- `results/`: Summary tables of identified similar compounds.

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/ParthivRajesh/Drug-Similarity-Analysis-AIP.git
   ```
2. Follow the instructions in the `workflow/README.md` to set up and execute the KNIME workflows.
3. Review the results and visualizations in their respective directories.
