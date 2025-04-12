**Unsupervised Machine Learning Framework for Clustering DNA Nucleotide Transmission Footprints**

This repository presents an unsupervised machine learning (ML) framework developed to cluster the transmission spectra of DNA nucleotides by identifying unique transmission "footprints" through feature-based analysis.

**Overview**

We constructed a generalized ML pipeline by extracting physically meaningful features from quantum transport transmission profiles of DNA nucleotides. Among these, the following were identified as highly effective for clustering:

**MIN**: Minimum normalized transmission value

**Height**: Difference between transmission values of two consecutive peaks

These features capture the essential shape and depth variations within transmission spectra, enabling better clustering performance.

**Clustering Techniques Used**

A variety of unsupervised ML algorithms were applied, including Prototype-based, Density-based, Hierarchical, and Soft Clustering. Out of all the methods tested, K-Medoids and Fuzzy C-Means produced the best clustering performance with:

**Silhouette Score**:~0.72

**Davies-Bouldin Index**: ~0.44

**Energy Window Refinement**

To enhance clustering clarity, we focused on a narrower energy range of ±1.5 eV around the Fermi level, where more distinct transmission peaks are observed.

This refinement led to significantly improved metrics:

**Silhouette Score**: ~0.83

**Davies-Bouldin Index**: ~0.40

This demonstrates that selecting an appropriate energy window strengthens the resolution of clustering.

**Repository Contents**

Features(complete energy range).xlsx – Features extracted ±2.5 eV of the Fermi level

Features(close to Fermi).xlsx – Features extracted within ±1.5 eV of the Fermi level

README.md – Project overview and usage guide

