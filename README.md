# CAEM-GBDT

Deep learning approach for cancer subtype classification using high-dimensional multi-omics data
It is built with **Tensorflow** and **Python 3**.


## Requirements

  * python 3.7, numpy, scipy, TensorFlow 2.12, pysam


## Codes

  * breast-gene.ipynb
  * breast-methy.ipynb
  * breast-mirna.ipynb
  * breast-multi-omics.ipynb
  * GBM-gene.ipynb
  * GBM-methy.ipynb
  * GBM-mirna.ipynb
  * GBM-multi-omics.ipynb


## Data

  * BRCA_clinicalMatrix.xls
  * BREAST_Gene_Expression.xls
  * BREAST_Methy_Expression.xls
  * BREAST_Mirna_Expression.xls
  * GBM_clinicalMatrix.xls
  * GLIO_Gene_Expression.xls
  * GLIO_Methy_Expression.xls
  * GLIO_Mirna_Expression.xls
  * The original dataset can be downloaded from https://github.com/tuiainao316/datasets


## Usage

### Data preprocessing

1. Manually save the .xls file as .csv, and then use the np.savetxt function to convert the .csv file to .txt.
2. Read the data (.txt), check the data and label dimensions,
3. Feature normalization before training

### Build the model

1. Change the shape according to different datasets in the model.build function
2. Set different structures for different datasets.

### Train Model

1. Set the loss function and evaluation indicators
2. Define the training and test steps
3. Defining and dividing the dataset
4. After the training steps, the model is finally evaluated on the test set.
