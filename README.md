# 🧠 Image Captioning System using Vision Transformer & GPT-2

## 📌 Overview

This project implements a deep learning-based **Image Captioning System** that automatically generates natural language descriptions for images.

The system combines:

- A **Vision Transformer (ViT)** as an image encoder
- A **GPT-2 Transformer** as a text decoder

The model is fine-tuned on the **Microsoft COCO 2017 dataset** and trained using PyTorch with mixed precision and advanced optimization strategies.

---

## 🚀 Key Features

- 🖼️ Automatic image caption generation
- 🔥 Vision Transformer + GPT-2 architecture (Encoder–Decoder)
- 📊 Fine-tuned on COCO 2017 dataset
- 🎯 Beam Search decoding for higher-quality captions
- 📉 Evaluation using BLEU, ROUGE-L, METEOR
- ⚡ Mixed Precision Training (AMP)
- 💾 Checkpoint saving & training resume support
- 📈 Cosine Annealing Learning Rate Scheduler
- 📊 Training visualization (loss & metrics curves)

---

## 📂 Dataset

### Microsoft COCO 2017 Dataset

**Used subsets:**

- Training: 50,000 images
- Validation: 2,000 images

**Includes:**

- train2017
- val2017
- captions_train2017.json
- captions_val2017.json

---

## 🧠 Model Architecture

### Encoder

- Vision Transformer (ViT)
- Extracts high-level visual features

### Decoder

- GPT-2 Transformer
- Generates natural language captions

### Full Pipeline

Image → ViT Encoder → Transformer Decoder (GPT-2) → Caption

---

## 🛠️ Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- COCO API (pycocotools)
- NumPy
- Matplotlib
- Evaluate (BLEU, ROUGE, METEOR)
- Google Colab

---

## ⚙️ Training Configuration

| Parameter             | Value            |
| --------------------- | ---------------- |
| Batch Size            | 8                |
| Gradient Accumulation | 4                |
| Learning Rate         | 2e-6             |
| Epochs                | 6                |
| Beam Size             | 5                |
| Max Caption Length    | 32               |
| Optimizer             | AdamW            |
| Scheduler             | Cosine Annealing |

---

## 📊 Evaluation Metrics

- BLEU Score → n-gram precision
- ROUGE-L → sequence matching quality
- METEOR → semantic similarity
- Token Overlap Accuracy

---

## 📈 Training Highlights

- Stable convergence across epochs
- Reduced loss via cosine learning rate decay
- Improved caption fluency using beam search
- Regular checkpoint saving to Google Drive

---

## 🧪 Example Output

**Input Image:**  
Any COCO-style image

**Generated Caption:**

> A group of people standing near a train station.

---

## 📁 Project Structure

Image-Captioning-System/
│
├── notebook/
│ └── image_captioning.ipynb
│
├── checkpoints/
│ └── model.safetensors
│
├── data/
│ └── COCO dataset
│
├── requirements.txt
└── README.md

---

## 👨‍💻 Author

**Maged Hujira**  
🎓 semester Project – Artificial Intelligence  
💡 Focus: Computer Vision & Natural Language Processing

---

## 🏁 Status

✔️ Project Completed  
✔️ Fully Trained & Evaluated  
✔️ Ready for Deployment / Demonstration
