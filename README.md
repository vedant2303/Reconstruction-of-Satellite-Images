# Reconstruction-of-Satellite-Images

## Overview

This repository contains the code and documentation for a project that focuses on converting satellite images into human-readable maps using a Conditional Generative Adversarial Network (cGAN). The goal is to reduce latency in map generation and improve data accessibility for various applications across domains.

## Project Description

### Problem Statement

Generating maps from satellite images is a valuable but time-consuming process across multiple domains, including E-automobile companies, food supply chains, E-commerce logistics, and intelligence agencies. The project addresses the challenge of automating this process to reduce latency between actual geographic views and publicly available human-readable maps.

### Dataset

The dataset used for training consists of 1096 concatenated satellite images paired with their respective map images. These images were collected from New York City Park using the Google Maps API. The original image size of 1200x600 was preprocessed and resized to 256x256 dimensions.

Dataset Download Link:  http://efrosgans.eecs.berkeley.edu/pix2pix/datasets/
Note: "Please click the following link to download the 'maps.tar.gz' dataset used in our project."

### Approach

- The project employs a Conditional GAN (cGAN) model for image-to-image translation, where a real satellite image is input into the generator to produce a fake map image.
- The generator is based on a modified U-net architecture for improved results.
- A new discriminator model, also modified from the PatchGAN architecture, enhances classification accuracy.

### Implementation

The project is implemented using Python and deep learning libraries such as TensorFlow and Keras. The training process includes optimizing the generator and discriminator models, with a focus on minimizing losses.

## Getting Started

Follow these steps to get started with the project:

1. Clone this repository: `git clone https://github.com/your-username/satellite-image-to-map-conversion.git`
2. Install the required dependencies listed in the `requirements.txt` file.
3. Run the training script to train the cGAN model.
4. Use the trained model for generating map images from satellite images.

## Results

The project achieved promising results, with the following average losses:

- L1 Loss: 0.084
- L2 Loss: 0.088
- GAN Loss: 13.181

## Conclusion

This project demonstrates the potential of using conditional GANs for automating the conversion of satellite images into human-readable maps. The modified architecture and training approach contribute to more robust results.
