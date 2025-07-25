# A Deep Learning Model Leveraging Semantic Features Fusion for DNase I Hypersensitive Sites Identification in the Human Genome
This repository contains resources related to the research titled **A Deep Learning Model Leveraging Semantic Features Fusion for DNase I Hypersensitive Sites Identification in the Human Genome** In this study, we propose various computational models, namely: CNN Model, CNN-GRU Fusion Model, CNN-Kmer Fusion Model, CNN-GRU-Kmer Fusion model, to overcome the challenges associated with DHSs prediction. In CNN Model based on a simple 1-dimensional CNN. In CNN-GRU Fusion Model, based on simple 1-dimensional CNN and GRU, then fused the feature maps of CNN and GRU. In CNN-Kmer Fusion Model, based on simple 1-dimensional CNN and Kmer features, first we input the kmer features to dense layer, the output of dense layer are fused with CNN features. In CNN-GRU-Kmer Fusion Model, based on simple 1-dimensional CNN, GRU and Kmer features, first we input the kmer features to dense layer, the output of dense layer is fused with CNN features and GRU features, and fed to dense layer with sigmoid function for prediction.

## Proposed Framework
## Proposed Framework
### Benchmark Dataset
This dataset consist of 280 DHS sequences and 737 non-DHS sequences [1], which could be freely downloaded from https://noble.gs.washington.edu/proj/hs/

### Feature Fusion Space
Feature extraction is a crucial step in designing and extracting information patterns from biological sequences. In this work, we employed various feature encoding methods:
-	**k-mer encoding**
- **One-hot encoding with CNN**
- **One-hot encoding with GRU**

### Proposed Model Framework
Framework of our proposed models: CNN Model, CNN-GRU Fusion Model, CNN-Kmer Fusion Model, CNN-GRU-Kmer Fusion Model

<p align="center">
<img src="https://github.com/malikmtahir/DNase/blob/main/architecture.jpg " width="500" height="800">
<p align="center">
System model of the proposed framework highlighting data, feature fusion, and model spaces

## Feature Visualization
To visualize the features, we use **t-SNE** to reduce the dimensionality of the **CNN features, GRU features, k-mer features, and Dense layer features** from the training set. This will allow us to see how the model's learned representations cluster and separate different data points in a 2D space, helping to interpret the feature learning process.

<p align="center">
<img src="https://github.com/malikmtahir/DNase/blob/main/t-sne.jpg" width="550" height="500">  <p align="right">


### Comparative Analyses against State-of-the-art Models
This comparative study evaluates the developed ensemble model against the cutting-edge model **Jin et al., [1]** focusing on theDNase I hypersensitive sites in the human genome problem.
  
### Statistical Analyses
The statistical analysis is based on the **standard error method** that computes the **mean, standard deviation, critical value** (i.e., **z-score**), and **95% confidence interval** for a sample of **accuracy, sensitivity, specificity, MCC,** and **AUC-ROC**. These analyses aim to validate the quantitative results against the all proposed models.

  
# References 
The following references are utlized in the comparative analyses.

[1]. Jin, Y.T., Tan, Y., Gan, Z.H., Hao, Y.D., Wang, T.Y., Lin, H. and Tang, B., 2024. Identification of DNase I hypersensitive sites in the human genome by multiple sequence descriptors. Methods, 229, pp.125-132.

# Contact details
## Muhammad Tahir (m.tahir@umanitoba.ca, muhammadtahir@awkum.edu.pk)
### Affiliation:
1. **Department of Electrical and Computer Engineering, University of Manitoba, Winnipeg, Manitoba, R3T5V6, Canada**
2. **Department of Computer Science, Abdul Wali Khan University, Mardan, Mardan, 23200, Pakistan**

