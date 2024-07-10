# Pixelated Image Detection and Correction

![Depixelation Example](https://github.com/nafis71041/pixelation_correction/blob/main/depixelation_examples/success4_protest_4x_lanczos_nearest.png)
*Pixelated image (left), depixelated by our model (middle), and the ground truth (right)*

## Problem Statement

Pixelation is a common issue in images, leading to a loss of quality and important details.It generally arises due to downscaling an image by some factor and then upscaling it using some interpolation method. The objective of this project is to develop models capable of detecting and depixelating images, restoring them to a higher quality while maintaining computational efficiency.

## Description

This repository contains two primary models: a [detector model](https://github.com/nafis71041/pixelation_correction/blob/main/detector_005_1_50.keras) to identify pixelated images and a [depixelator model](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_004_2.keras) to restore pixelated images to their original quality. Both models were inspired by the U-Net architecture but optimized for efficiency using depthwise and pointwise convolutions.

## Repository Structure

### Project Report
- **[Project Report.pdf](https://github.com/nafis71041/pixelation_correction/blob/main/Project%20Report.pdf)**

Project report can be found here.

### Testing Files
- **[detector_testing.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/detector_testing.ipynb)**
- **[depixelator_testing.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_testing.ipynb)**

These are the testing files. Users should follow the instructions in these files to test our detector and depixelator models.

**Step-by-Step Guide to Test Our Models**

1. **Update and Import Libraries:** Ensure all required libraries are updated to the necessary versions and import them.

2. **Load the Models:** Load the pre-trained detector or depixelator model.

3. **(Important) Implement the TODO Cell:** Complete the `TODO` cell according to your own dataset, defining `image_paths` and `image_labels` or `pixelated_image_paths`, and optionally `real_image_paths`.

4. **Test the Model:** Follow the steps provided in the testing files to effectively test the models on your dataset.

### Training Files
- **[detector_training.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/detector_training.ipynb)**
- **[depixelator_training.ipynb](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_training.ipynb)**

These are the training files used for our detector and depixelator models. They are included for reference to show how we trained our models.

### Model Architectures
- **[detector_005_1.png](https://github.com/nafis71041/pixelation_correction/blob/main/detector_005_1.png)**
- **[depixelator_004_2.png](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_004_2.png)**

These images depict the detailed architectures of our models.

### Pre-trained Models
- **[detector_005_1_50.keras](https://github.com/nafis71041/pixelation_correction/blob/main/detector_005_1_50.keras)**
- **[depixelator_004_2.keras](https://github.com/nafis71041/pixelation_correction/blob/main/depixelator_004_2.keras)**

These files contain the pre-trained models with their corresponding architectures.

### Depixelation Examples
- **[Depixelation Examples](https://github.com/nafis71041/pixelation_correction/tree/main/depixelation_examples)**

This folder contains some successful and unsuccessful depixelation examples from our model.

## Conclusion

This repository offers a comprehensive solution for detecting and depixelating images, utilizing state-of-the-art techniques for efficiency and accuracy. By following the provided instructions and completing the required steps, users can effectively apply these models to their datasets to achieve high-quality image restoration.

For any questions or issues, please feel free to open an issue on this repository.
