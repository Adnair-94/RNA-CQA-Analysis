# RNA-CQA-Analysis

This repository contains R scripts used for data visualization and statistical analysis of
key performance indicators (KPIs) and critical quality attributes (CQAs) in the study:

“Integrated in vitro transcription–oligo-dT chromatography enables reagent recycling
for sustainable high-quality mRNA manufacturing”

The scripts reproduce figures and extended data panels using replicate-level source data
provided in the Supplementary Information and Supplementary Data of the manuscript.

---

## Repository scope

The analyses in this repository cover:

- Process KPIs (yield, recovery, productivity, cost-related metrics)
- RNA integrity and poly(A) tail heterogeneity
- 5′ capping efficiency and dsRNA content
- Cell-based functional assays (transfection efficiency and cytokine response)

The code is intended for transparency and reproducibility of the published results rather
than as a general-purpose or production-ready analysis pipeline.

---

## Repository structure

Scripts are organized by analysis type:

- `KPI_analysis/`  
  Yield, recovery, productivity, and cost-related plots (Figures 2–3).

- `Integrity_PolyA/`  
  RNA integrity and poly(A) tail heterogeneity analysis (Figure 4 and Extended Data).

- `Capping_dsRNA/`  
  5′ capping efficiency and dsRNA quantification (Figure 5).

- `Cell_Assays/`  
  Transfection efficiency and cytokine analysis (Figure 6).

Supporting helper functions may be placed in subfolders within each directory.

Output figures are written to the corresponding script folders or to an `output/` subdirectory.

---

## Requirements

- R version ≥ 4.2.0
- R packages commonly used include:
  - tidyverse
  - ggplot2
  - patchwork
  - rstatix
  - readxl
  - cowplot

Exact package versions used during manuscript preparation can be obtained via
`sessionInfo()`.

---
Input data

The scripts are designed to operate on replicate-level source data provided in the
manuscript Supplementary Information and Supplementary Data files.

Raw instrument files (e.g., electropherograms or LC–MS files) are not required to reproduce
the figures reported in the manuscript.

Where necessary, file paths within scripts may need to be updated to match local data
locations.

---
2. Open the relevant script in RStudio.

3. Set the working directory to the script location.

4. Run the script to generate the corresponding figures.
Output files are saved locally by each script.

---

## Reproducibility

All statistical analyses were performed using independent biological replicates (n = 3),
with statistical tests as described in the manuscript Methods section.

Given the same input data, the scripts deterministically reproduce the reported figures and
summary statistics.

---

## License

This repository is provided for academic and non-commercial use.
A license file may be added in future revisions.

---

## Citation

If you use this code, please cite the associated manuscript.


