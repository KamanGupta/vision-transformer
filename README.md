# Vision Transformer (ViT) from Scratch on CIFAR-10

A PyTorch implementation of a Vision Transformer (ViT) built from scratch for image classification on the CIFAR-10 dataset.

## Project Overview

This project implements the Vision Transformer architecture by treating images as sequences of patches and applying multi-head self-attention for feature extraction and classification.

Unlike traditional CNNs, Vision Transformers leverage transformer-based architectures originally developed for NLP tasks, enabling global feature interactions through self-attention mechanisms.

## Dataset

- CIFAR-10
- 60,000 RGB images
- 10 object classes
- Image size: 32 × 32

Classes:
- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

## Model Architecture

### Patch Embedding
- Image Size: 32 × 32
- Patch Size: 4 × 4
- Number of Patches: 64

### Transformer Encoder
- Embedding Dimension: 256
- Number of Encoder Layers: 6
- Attention Heads: 8
- Feed Forward Dimension: 512
- Dropout: 0.1

### Classification Head
- CLS Token
- Layer Normalization
- Fully Connected Layer

## Training Configuration

| Parameter | Value |
|------------|--------|
| Optimizer | AdamW |
| Learning Rate | 1e-3 |
| Scheduler | Cosine Annealing |
| Batch Size | 128 |
| Epochs | 30 |
| Loss Function | Cross Entropy |

## Data Augmentation

- Random Horizontal Flip
- Random Crop
- Normalization

## Results

| Metric | Value |
|---------|---------|
| Training Accuracy | 71.18% |
| Test Accuracy | 69.95% |

## Key Features

- Custom Patch Embedding Layer
- Multi-Head Self-Attention
- Positional Encoding
- Transformer Encoder Blocks
- AdamW Optimization
- Cosine Learning Rate Scheduling
- Data Augmentation Pipeline

## Repository Structure
