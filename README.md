# MiniGPT From Scratch

A simplified implementation of a GPT-style language model built entirely from scratch using PyTorch. This project follows the core ideas behind decoder-only Transformers and demonstrates how modern Large Language Models generate text.

The model is trained on the Tiny Shakespeare dataset and learns to predict the next character in a sequence using self-attention and autoregressive language modeling.

---

## Features

- Character-level tokenization
- Custom vocabulary creation
- Train/validation dataset split
- Batch generation pipeline
- Bigram language modeling
- Transformer-based architecture
- Multi-Head Self-Attention
- Positional Embeddings
- Feed Forward Networks
- Residual Connections
- Layer Normalization
- Autoregressive Text Generation
- PyTorch implementation from scratch

---

## Project Structure
MiniGPT-From-Scratch/
│
├── MiniGPT.ipynb
├── input.txt
└── README.md

---

## Dataset

The model is trained on the Tiny Shakespeare dataset, a popular benchmark used for learning language modeling concepts.

Dataset Source:
https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt

---

## Model Pipeline

### 1. Data Preparation

- Load text dataset
- Build vocabulary
- Create character-to-index mapping
- Encode text into token IDs

### 2. Dataset Splitting

- 90% Training Data
- 10% Validation Data

### 3. Batch Generation

Random context windows are sampled during training to create input-target pairs.

### 4. Transformer Architecture

The model includes:

- Token Embeddings
- Positional Embeddings
- Multi-Head Masked Self-Attention
- Feed Forward Network
- Residual Connections
- Layer Normalization

### 5. Training

The model is trained using:

- Cross Entropy Loss
- AdamW Optimizer
- Backpropagation through Transformer blocks

### 6. Text Generation

After training, the model generates text autoregressively by repeatedly predicting the next token.

---

## Technologies Used

- Python
- PyTorch
- NumPy
---

## Learning Outcomes

This project demonstrates:

- Language Modeling Fundamentals
- Transformer Architecture
- Self-Attention Mechanism
- GPT Decoder Design
- Token Embeddings
- Positional Encoding
- Sequence Modeling
- Neural Text Generation

---

## Future Improvements

- Byte Pair Encoding (BPE) Tokenization
- Larger Transformer Architectures
- GPT-2 Style Implementation
- Mixed Precision Training
- Fine-Tuning on Custom Datasets
- Distributed Training
