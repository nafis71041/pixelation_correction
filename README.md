# Depixelator and Detector Models

![Depixelation Example](https://github.com/nafis71041/pixelation_correction/blob/main/depixelation_examples/success4_protest_4x_lanczos_nearest.png)
An exemplary collage image of a pixelated image, depixelated by our model, and the ground truth.

## Description

This repository contains two primary models: a [detector model](https://github.com/nafis71041/pixelation_correction/blob/main/detector_005_1_50.keras) to identify pixelated images and a [depixelator model](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_004_2.keras) to restore pixelated images to their original quality. Both models were inspired by the U-Net architecture but optimized for efficiency using depthwise and pointwise convolutions.

### Problem Statement

Pixelation is a common issue in images, leading to a loss of quality and important details. The objective of this project is to develop models capable of detecting and depixelating images, restoring them to a higher quality while maintaining computational efficiency.

## Repository Structure

- **[depixelator_004_2.keras](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_004_2.keras)**: Contains the architecture and pre-trained weights of the depixelator model.
- **[detector_005_1_50.keras](https://github.com/nafis71041/pixelation_correction/blob/main/detector_005_1_50.keras)**: Contains the architecture and pre-trained weights of the detector model.
- **[detector_training.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/detector_training.ipynb)  and [depixelator_training.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_training.ipynb)**: Includes scripts and notebooks used to train both the detector and depixelator models.
- **[detector_testing.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/detector_testing.ipynb) and [depixelator_testing.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_testing.ipynb)**: Includes scripts and notebooks for testing the models on user-provided datasets.
- **[detector_005_1.png](https://github.com/nafis71041/pixelation_correction/blob/main/detector_005_1.png) and [depixelator_004_2.png](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_004_2.png)**: Contains images depicting the architectures of the detector and depixelator models.


# Repository Overview

## Training Files
The [detector_training.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/detector_training.ipynb) and [depixelator_training.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_training.ipynb) files contains all the necessary scripts and notebooks used during the model training process. These files serve as a reference to provide insight into the training procedures. Users are encouraged to review these files to understand the methodologies and potentially modify or extend the models.

## Testing Files
The [detector_testing.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/detector_testing.ipynb) and [depixelator_testing.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_testing.ipynb) files contains includes detailed scripts and notebooks designed to test the models on user-provided datasets. Each file contains step-by-step instructions on how to load the pre-trained models and perform testing.

## Steps to Test Models

1. **Load the Pre-trained Models**
   The testing scripts will guide you through the process of loading the pre-trained models for both detection and depixelation tasks.

2. **Prepare Your Dataset**
   - For the detector model, prepare two lists: `image_paths` and `image_labels`.
   - For the depixelator model, prepare `pixelated_image_paths` and optionally `real_image_paths`.

3. **Implement TODO Cells**
   Each testing file includes `TODO` cells where users must define the paths to their images and labels based on their test dataset organization. Proper completion of these cells is essential for the scripts to access and process the data correctly.

## Important Note

Ensure that you correctly define the `image_paths`, `image_labels`, `pixelated_image_paths`, and `real_image_paths` lists in the provided `TODO` cells. This step is critical for the scripts to function correctly with your dataset.

## Conclusion

This repository offers a comprehensive solution for detecting and depixelating images, utilizing state-of-the-art techniques for efficiency and accuracy. By following the provided instructions and completing the `TODO` cells, users can effectively apply these models to their datasets to achieve high-quality image restoration.

For any questions or issues, please feel free to open an issue on this repository.
