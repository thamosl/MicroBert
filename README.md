# Mini-BERT

A lightweight **BERT model trained from scratch** using the WikiText-103 dataset and Hugging Face Transformers.

## Overview

This project implements a compact BERT architecture and pre-trains it using:

* **Masked Language Modeling (MLM)**
* **Next Sentence Prediction (NSP)**

The goal is to understand and experiment with the BERT pretraining process using a smaller model.

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

Install the dependencies:

```bash
pip install torch transformers datasets huggingface_hub
```

Then open and run:

```text
Micro_Bert.ipynb
```

## Model

The trained model can be saved locally and uploaded to the Hugging Face Hub for later use.

## Author

**Thamotharan**
**tharanthamo018@gmail.com
