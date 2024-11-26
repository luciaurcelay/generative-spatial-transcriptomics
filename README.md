# Multimodal VAE for Synthetic Spatial Transcriptomics Data

This project implements a multimodal Variational Autoencoder (VAE) designed to generate synthetic spatial transcriptomics (ST) data. By leveraging a graph neural network (GNN) for spatial transcriptomics, a vision transformer (H-Optimus-0) for whole slide images (WSIs), and a fully connected network (FCN) for metadata, the model enables controllable generation of new data. **The project is currently under active development.**

![st vae](https://github.com/user-attachments/assets/5b6f8d8e-08de-449e-9f9b-4a230ae06c1b)

## Motivation
Advances in spatial transcriptomics have enabled the understanding of spatially resolved gene expression in tissues. However, generating high-quality spatial transcriptomics datasets remains expensive and time-intensive. This project aims to develop a model for controllable synthetic data generation, which could:

- Facilitate data augmentation for model training.
- Enable the exploration of hypothetical scenarios in tissue organization and gene expression.
- Advance downstream applications such as digital pathology, disease modeling, and multi-modal data integration

## Features
- Graph Neural Network Encoder for ST: Encodes spatial relationships of gene expression data, capturing local and global structures within the tissue.
- Vision Transformer Encoder (H-Optimus-0): Extracts semantic features from histological whole-slide images.
- Metadata Encoder: Encodes structured metadata (e.g., organ, disease state) into a learnable embedding.
- Controllable Data Generation: Latent space allows for interpolation and exploration of new synthetic spatial transcriptomics datasets.
