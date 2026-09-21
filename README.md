# Mini-BERT

A lightweight **BERT model trained from scratch** using the WikiText-103 dataset and Hugging Face Transformers.

## Overview

This project implements a compact BERT architecture and pre-trains it using:

* **Masked Language Modeling (MLM)**
* **Next Sentence Prediction (NSP)**

The project is designed to understand and experiment with the BERT pretraining process using a smaller model.

## Pretrained Model

The trained model is available on Hugging Face:

🤗 **[Thamo31/MiniEmbedding](https://huggingface.co/Thamo31/MiniEmbedding)**

## Model Configuration

| Parameter           | Value |
| ------------------- | ----: |
| Hidden Size         |   256 |
| Transformer Layers  |     4 |
| Attention Heads     |     4 |
| Max Sequence Length |   128 |
| Training Epochs     |     3 |
| Batch Size          |    16 |
| Learning Rate       |  5e-4 |

## Tech Stack

* Python
* PyTorch
* Hugging Face Transformers
* Hugging Face Datasets
* WikiText-103
* CUDA / GPU

## Training Pipeline

```text
WikiText-103
     ↓
Text Preprocessing
     ↓
Sentence Pair Creation
     ↓
BERT Tokenization
     ↓
MLM + NSP
     ↓
Mini-BERT Training
     ↓
Saved Model
```

## Run the Project

Install the required packages:

```bash
pip install torch transformers datasets huggingface_hub
```

Open and run:

```text
Micro_Bert.ipynb
```

## Author

**Thamotharan**
AI & Data Science
