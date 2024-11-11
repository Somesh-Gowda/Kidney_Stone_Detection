# Kidney_Stone_Detection

This project is a simple pipeline for detecting kidney stones in grayscale images using basic image processing techniques in Python. The code is aimed at detecting regions that could potentially indicate kidney stones, based on applying several image filters and thresholding methods.

## Overview

The pipeline includes several main stages:
1. **Histogram Equalization**: Enhances contrast in grayscale images.
2. **Gaussian Filter**: Smooths the image and reduces noise.
3. **Median Filter**: Further reduces noise, especially "salt-and-pepper" noise.
4. **Laplacian Filter**: Enhances edges in the image to help identify regions of interest.
5. **Morphological Segmentation**: Using erosion and dilation, regions are segmented to isolate possible stones.
6. **Otsu Thresholding**: Separates the image into binary regions to further isolate high-contrast areas.

## Requirements

- Python 3.x
- OpenCV
- Matplotlib
- Scikit-image

## Installation

Install the necessary libraries by running:

pip install opencv-python-headless matplotlib scikit-image

## Usage
Add a grayscale image (preferably a kidney scan) in the path specified in the code.
Run the code:

python kidney_stone_detection.py
