# Egyptian License Plate Recognition

This repository implements an end-to-end pipeline for **Egyptian License Plate Recognition**, utilizing advanced computer vision techniques and deep learning models.

## Project Description

The system is designed to detect and recognize Egyptian license plates from images or video feeds. It integrates **YOLO** for license plate detection and **TrOCR** for Optical Character Recognition (OCR), with preprocessing steps tailored to Arabic script.

## Features

1. **Object Detection:**
   - YOLO is used to locate license plates in input images.
2. **Optical Character Recognition (OCR):**
   - TrOCR from the Hugging Face Transformers library processes and extracts textual information.
3. **Arabic Script Recognition:**
   - Support for Arabic and alphanumeric characters specific to Egyptian license plates.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/SandyHedia/Egyptian-License-Plate-Recognition.git
   cd Egyptian-License-Plate-Recognition
   ```

2. Install the required dependencies:
  
   run the setup commands from the notebooks to install packages:
   - `ultralytics`
   - `transformers`
   - `torch`
   - `opencv-python`

3. Download and prepare the dataset:
   - Ensure your dataset is structured appropriately (e.g., images and corresponding labels).
   - Place it in the `data/` directory or update the paths in the scripts.

## Usage

### Training

- **Object Detection Model (YOLO):**
  - Train YOLO on the license plate dataset to detect license plate regions.

- **OCR Model (TrOCR):**
  - Fine-tune TrOCR for recognizing Arabic characters.

### Inference

- Detect license plates and recognize characters in an image.

### Evaluation

Evaluate the models on a test set to determine detection and recognition accuracy.

## Dataset

- Custom dataset of Egyptian license plates with bounding box annotations and character labels.
- Preprocessing includes image resizing, normalization, and augmentation.
