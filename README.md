# PLDBench: Benchmarking of Different Molecular Docking Methods for Protein–Peptide Docking

## Overview

PLDBench is a benchmarking framework developed for evaluating the performance of different molecular docking methods used in protein–peptide docking studies.

Protein–peptide interactions are essential in many biological processes including:

- Immune response
- Cell signaling
- Apoptosis
- Cellular localization
- Therapeutic peptide design

The study benchmarked six widely used docking methods on a large dataset of experimentally validated protein–peptide complexes.

The performance evaluation was carried out using CAPRI parameters:

- FNAT
- I-RMSD
- L-RMSD

A web-based platform named **PPDbench** was also developed for benchmarking docking methods and calculating CAPRI parameters.

---

# Research Paper

## Title

Benchmarking of Different Molecular Docking Methods for Protein–Peptide Docking

## Authors

- Piyush Agrawal
- Harinder Singh
- Hemant Kumar Srivastava
- Sandeep Singh
- Gaurav Kishore
- Gajendra P. S. Raghava

## Journal

BMC Bioinformatics

## Published Year

2019

## DOI

https://doi.org/10.1186/s12859-018-2449-y

## Source Paper



---

# Background

Protein–peptide interactions constitute nearly 40% of all macromolecular interactions.

Peptides are highly flexible molecules and can adopt numerous conformations, making docking studies highly challenging.

Several docking tools exist for:

- Protein–protein docking
- Protein–ligand docking
- Protein–peptide docking

However, only limited benchmarking studies had previously been performed specifically for protein–peptide complexes.

This study aimed to rigorously benchmark major docking methods using a large and diverse dataset.

---

# Objectives

The main objectives of the study were:

- Benchmark different docking methods
- Evaluate blind docking performance
- Evaluate re-docking performance
- Assess scoring functions
- Analyse docking reproducibility
- Study the effect of molecular properties on docking quality
- Develop a benchmarking platform for the scientific community

---

# Docking Methods Evaluated

The following six docking methods were benchmarked:

| Docking Method | Type |
|---|---|
| ZDOCK 3.0.2 | Protein–protein docking |
| FRODOCK 2.0 | Protein–protein docking |
| Hex 8.0.0 | Protein–protein docking |
| PatchDock 1.0 | Geometric docking |
| ATTRACT | Flexible docking |
| pepATTRACT | Protein–peptide docking |

Source: :contentReference[oaicite:1]{index=1}

---

# Dataset Information

## Main Dataset: PPDbench

The benchmark dataset consisted of:

- 133 non-redundant protein–peptide complexes
- Peptide length between 9–15 residues
- Less than 40% sequence similarity

The dataset was generated using:

- peptiDB dataset
- ACCLUSTER dataset

Redundancy removal was performed using:

- CD-HIT


---

# CAPRI Evaluation Parameters

The docking methods were evaluated using standard CAPRI parameters:

## FNAT

Fraction of native contacts preserved in the docked structure.

## I-RMSD

Interface Root Mean Square Deviation.

## L-RMSD

Ligand Root Mean Square Deviation.

---

# Blind Docking Analysis

Blind docking was performed without prior binding site information.

## Top Docking Pose Performance

### Best Method

FRODOCK performed best among all methods.

| Parameter | Value |
|---|---|
| Average L-RMSD | 12.46 Å |

## Best Docking Pose Performance

FRODOCK again achieved the best performance.

| Parameter | Value |
|---|---|
| Average L-RMSD | 3.72 Å |



---

# Re-Docking Analysis

Re-docking was performed using binding-site information.

## Best Performing Method

ZDOCK achieved the best performance.

### Top Pose

| Parameter | Value |
|---|---|
| Average L-RMSD | 8.60 Å |

### Best Pose

| Parameter | Value |
|---|---|
| Average L-RMSD | 2.88 Å |


---

# Important Findings

## FRODOCK

- Best method for blind docking
- Efficient rotational search using spherical harmonics
- Excellent scoring performance

## ZDOCK

- Best method for re-docking
- FFT-based docking algorithm
- Better performance with known binding sites

## pepATTRACT

- Lowest performance among tested methods
- Performance affected by peptide structure prediction quality

---

# Scoring Function Analysis

The study found that:

- Current scoring functions are insufficient for ranking docking poses accurately
- Best docking poses are often not ranked as top poses
- Universal scoring functions are required

FRODOCK demonstrated the best scoring capability among evaluated methods.

---

# Reproducibility Analysis

Docking reproducibility was tested by repeating docking experiments.

Results showed:

- Most methods produced nearly identical results
- Docking methods are highly reproducible



---

# Secondary Structure Analysis

Docking methods performed better on:

- Coiled peptides

Compared to:

- Regular secondary structure peptides
- Helical peptides
- Sheet-containing peptides

Possible reason:

- Higher flexibility of coiled peptides

---

# Resolution Analysis

Protein–peptide complexes with:

- Higher crystal structure resolution (1–2 Å)

Produced better docking performance compared to:

- Lower resolution structures (2–3 Å)

---

# Rotatable Bond Analysis

The number of rotatable bonds significantly affected docking quality.

Key observations:

- Flexible peptides are harder to dock
- FRODOCK and ZDOCK handled flexibility better than other methods

---

# PPDbench Web Server

A web-based platform named **PPDbench** was developed.

## Features

### Single Mode

- Evaluate one docked complex

### Batch Mode

- Evaluate multiple complexes simultaneously

### Dataset Download

- Benchmark datasets available for download

### CAPRI Parameter Calculation

- FNAT
- I-RMSD
- L-RMSD

Web Server:

http://webs.iiitd.edu.in/raghava/ppdbench/

Source: :contentReference[oaicite:6]{index=6}

---

# Applications

PLDBench and PPDbench can be used for:

- Protein–peptide docking evaluation
- Benchmarking new docking algorithms
- Drug discovery
- Peptide therapeutic design
- Structural bioinformatics
- Molecular interaction studies

---

# Technologies Used

- CAPRI evaluation framework
- FFT docking algorithms
- Spherical harmonics
- CD-HIT
- Molecular docking algorithms
- Flexible docking methods

---

# Conclusion

The study concluded that:

- FRODOCK performs best for blind docking
- ZDOCK performs best for re-docking
- Current scoring functions need improvement
- Combining multiple docking methods improves docking success
- High-quality benchmark datasets are essential for future docking research

---

# Contact

## Dr. G. P. S. Raghava

Email: raghava@iiitd.ac.in

Address:  
Indraprastha Institute of Information Technology Delhi

---

# License

This work is distributed under the Creative Commons Attribution 4.0 International License.

---

