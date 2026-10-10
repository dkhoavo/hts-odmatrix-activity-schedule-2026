# Simulation Pipeline for Activity Schedule Reconstruction

This repository contains a transparent and reproducible pipeline for reconstructing activity schedules through simulation.

> **Before running the pipeline:** Update the file paths in the notebooks to match the locations of your input data and output folders.

## Repository structure

- `result_re1_release.ipynb`  
  Contains simulation outputs, intermediate results, and figures.

- `tour_gen_encoder_re1_release.ipynb`  
  Generates the Singapore and Seoul activity schedules reported in the manuscript. This notebook is provided for transparency.

- `val_tour_gen_encoder_re1_release.ipynb`  
  Generates activity schedules for the controlled experiments reported in the manuscript. The simulated data are provided in the `data` folder.

## Run the controlled experiment

In `val_tour_gen_encoder_re1_release.ipynb`, run the notebook sections in this order:

1. **Stage 1: Finding the number of latent classes**  
   Run this section to identify the best number of latent classes.

2. **Stage 1: Model Embedding** and **Stage 1: Data Fusion**  
   Run these sections to perform data fusion.

3. **Stage 2: Tour Generation**  
   Run this section to generate tours.

4. **Construct Activity Schedules**  
   Use the generated tours to construct activity schedules for the segregation analysis.

5. **Place Segregation**  
   Run this section to calculate place segregation.

6. **Individual Segregation**  
   Run this section to calculate individual segregation.

## Validate the controlled-experiment results

In `result_re1_release.ipynb`, run the following sections to validate the results:

1. **Validate Schedule** — validates the generated schedules.
2. **Validate Place Segregation** — validates place-level segregation.
3. **Validate Individual Segregation** — validates individual-level segregation.
