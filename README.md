# Image Captioning System using Vision Transformer and GPT-2

## Overview

This project implements an Image Captioning System using a Vision Transformer (ViT) encoder and GPT-2 decoder architecture. The model automatically generates natural language descriptions for images by combining computer vision and natural language processing techniques.

The project is based on the pre-trained `nlpconnect/vit-gpt2-image-captioning` model and was further trained and evaluated on the Microsoft COCO 2017 dataset.

---

## Features

* Automatic image caption generation
* Transfer learning using Vision Transformer (ViT) and GPT-2
* Fine-tuning on the COCO 2017 dataset
* Beam Search decoding for improved caption quality
* Evaluation using BLEU, ROUGE-L, and METEOR metrics
* Mixed Precision Training (AMP) for faster training
* Checkpoint saving and training resumption support
* Learning rate scheduling using Cosine Annealing

---

## Dataset

### Microsoft COCO 2017

The project uses:

* COCO Train2017
* COCO Validation2017
* COCO Caption Annotations

Training subset:

* 50,000 images

Validation subset:

* 2,000 images

---

## Model Architecture

Encoder:

* Vision Transformer (ViT)

Decoder:

* GPT-2 Language Model

Pretrained Model:

* nlpconnect/vit-gpt2-image-captioning

---

## Technologies Used

* Python
* PyTorch
* Hugging Face Transformers
* COCO API
* NumPy
* Matplotlib
* Evaluate
* NLTK

---

## Training Configuration

* Batch Size: 8
* Gradient Accumulation: 4
* Learning Rate: 2e-6
* Epochs: 6
* Beam Size: 5
* Maximum Caption Length: 32

---

## Evaluation Metrics

The model is evaluated using:

* BLEU
* ROUGE-L
* METEOR
* Token Overlap Accuracy

---

## Example Output

Input Image:

[Sample Image]

Generated Caption:

"A group of people standing near a train station."

---

## Project Structure

```text
Image-Captioning-System/
│
├── notebook/
│   └── sems_p.ipynb
│
├── docs/
│   ├── sems_project.pdf
│   └── presentation.pptx
│
├── data/
│   └── captions.txt.zip
│
├── requirements.txt
└── README.md
```

---

## Author

Maged Hujira

Semester Project – Artificial Intelligence
