 **# Image Captioning with Flickr8k**

## Overview

This repository contains the code and model for an image captioning project that generates natural language descriptions of images using the Flickr8k dataset.

## Dataset

* **Dataset:** Flickr8k
* **Source:** Kaggle: [https://www.kaggle.com/ming666/flicker8k-dataset](https://www.kaggle.com/ming666/flicker8k-dataset)
* **Description:** Contains 8,000 images with five crowd-sourced captions for each image.

## Structure

```
image-captioning/
├── README.md    # This file
├── data/       # Directory for storing the dataset
│   ├── Flickr8k_Dataset/       # Images
│   └── Flickr8k_text/          # Captions
├── models/     # Directory for saving trained models
├── src/        # Source code for the project
│   ├── data_loader.py        # Data loading and preprocessing
│   ├── model.py              # Model architecture
│   └── train.py              # Training script
└── requirements.txt   # List of required python packages
```

## Installation

1. Clone the repository:

```bash
git clone https://github.com/<your-username>/image-captioning.git
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

## Usage

1. Download the Flickr8k dataset from Kaggle and place it in the `data/` directory.
2. Train the model:

```bash
python src/train.py
```

3. Generate captions for images:

```bash
python src/generate_captions.py <path_to_image>
```

## Model Architecture

* **Image Encoder:** Pre-trained InceptionV3 model for image feature extraction.
* **Caption Decoder:** LSTM with attention mechanism for generating captions.

## Evaluation

* **BLEU score:** 0.46 (on the test set)

## Future Work

* Experiment with different model architectures (e.g., transformer-based models).
* Explore attention mechanisms for better caption generation.
* Incorporate beam search decoding for diverse captions.

## References

* Paper on Image Captioning with Attention: [https://arxiv.org/abs/1502.03044](https://arxiv.org/abs/1502.03044)
* Keras Tutorial on Image Captioning: [https://www.tensorflow.org/tutorials/text/image_captioning](https://www.tensorflow.org/tutorials/text/image_captioning)

## Contributing

Feel free to contribute to this project!

**[Kunal Lunia]**

**[26/12/2023]**
