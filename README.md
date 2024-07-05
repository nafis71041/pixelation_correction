# Depixelator and Detector Models

![Example Image](depixelation_examples/protest_d4_collage.jpg)  
An exemplary collage image of a pixelated image, depixelated by our model, and the ground truth.

## Description

This repository contains two primary models: a [detector model](https://github.com/nafis71041/pixelation_correction/blob/main/detector_005_1_50.keras) to identify pixelated images and a [depixelator model](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_004_2.keras) to restore pixelated images to their original quality. Both models were inspired by the U-Net architecture but optimized for efficiency using depthwise and pointwise convolutions.

### Problem Statement

Pixelation is a common issue in images, leading to a loss of quality and important details. The objective of this project is to develop models capable of detecting and depixelating images, restoring them to a higher quality while maintaining computational efficiency.

## Repository Structure

- **[depixelator_model](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_004_2.keras)**: Contains the architecture and pre-trained weights of the depixelator model.
- **[detector_model](https://github.com/nafis71041/pixelation_correction/blob/main/detector_005_1_50.keras)**: Contains the architecture and pre-trained weights of the detector model.
- **[training_files_detector] [training_files_depixelator]**: Includes scripts and notebooks used to train both the detector and depixelator models.
- **[testing_files_detector] [testing_files_depixelator]**: Includes scripts and notebooks for testing the models on user-provided datasets.
- **[detector_005_1.png](https://github.com/nafis71041/pixelation_correction/blob/main/detector_005_1.png)**: Contains images depicting the architectures of the detector and depixelator models.

## How to Use This Repository

### Training Files

The training_files directory contains all necessary scripts and notebooks used during the training of the models. These files are provided for reference and should give insight into the model training process. Users are encouraged to review these files to understand the training procedures and potentially modify or extend the models.

### Testing Files

The testing_files directory includes detailed scripts and notebooks to test the models on your own datasets. Each file contains step-by-step instructions on how to load the pre-trained models and perform testing. 

#### Steps to Test Models:

1. *Load the Pre-trained Models*:
   The testing scripts will guide you through loading the pre-trained models for both detection and depixelation tasks.

2. *Prepare Your Dataset*:
   - For the detector model, prepare two lists: image_paths and image_labels.
   - For the depixelator model, prepare pixelated_image_paths and optionally real_image_paths.

3. *Implement TODO Cells*:
   Each testing file has TODO cells where you must define the paths to your images and labels according to how your test dataset is organized. These cells are crucial for the scripts to correctly access and process your data.


### Note

- *Implement the TODO Cells*:
  Make sure to correctly define the image_paths, image_labels, pixelated_image_paths, and real_image_paths lists in the provided TODO cells. This is essential for the scripts to function properly with your dataset.

## Conclusion

This repository provides a comprehensive solution to detect and depixelate images, utilizing state-of-the-art techniques for efficiency and accuracy. By following the provided instructions and modifying the TODO cells, users can effectively use these models on their own datasets to achieve high-quality image restoration.

For any questions or issues, please feel free to open an issue on this repository.
