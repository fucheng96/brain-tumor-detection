## Table of Contents

1. [Overview](#Overview)
2. [Installation](#Installation)
3. [Folder Directory](#Folder-Directory)
4. [Acknowledgements](#Acknowledgements)

## Overview

The main objective of this project is to accurately classify whether a brain tumor is present in MRI images.<br>

3 Convolutional Neural Network models were developed:
1. Self-Built CNN Model
2. ResNet 50 Pre-trained (Transfer Learning)
3. VGG16 Pre-trained (Transfer Learning)

In the end, ranking of the models with accuracy on hold-out dataset is as follows:
1. **Self-Built CNN Model - 86% accuracy**
2. **VGG16 - 80% accuracy**
3. **ResNet50 - 63% accuracy**

More details can be found in the [Jupyter Notebook here](https://github.com/fucheng96/brain-tumor-detection/blob/main/brain-tumor-detection.ipynb).

## Installation

Clone this git repository to your local workspace.

`[https://github.com/fucheng96/brain-tumor-detection.git](https://github.com/fucheng96/brain-tumor-detection.git)`

## Folder Directory

- [brain-tumor-dataset](https://github.com/fucheng96/brain-tumor-detection/tree/main/data)<br>
  Consists of brain MRI images in various folders. 
   - yes - Contains 155 MRI images with brain tumor
   - no - Contains 98 MRI images with no tumor
   - train - Contains MRI images for model training, folder named '0' indicates no brain tumor and '1' indicators otherwise
   - valid - Contains MRI images for model validation, folder named '0' indicates no brain tumor and '1' indicators otherwise
   - test - Contains MRI images as hold-out dataset for model testing, folder named '0' indicates no brain tumor and '1' indicators otherwise  
- [brain-tumor-detection.ipynb](https://github.com/fucheng96/brain-tumor-detection/blob/main/brain-tumor-detection.ipynb)<br>
  This notebook contains all the details of this project from Problem Statement and Strategy to Exploratory Data Analysis. 
- [self_built_cnn_model.pt](https://github.com/fucheng96/brain-tumor-detection/blob/main/self_built_cnn_model.pt))<br>
  Self-built CNN pytorch model.

## Acknowledgements

Kudos to Navoneel Chakrabarty for releasing [brain MRI images](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection). It contains MRI images with and without tumor for detection purposes.
