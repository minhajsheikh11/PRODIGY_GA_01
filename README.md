# GPT-2 Text Generation 

## Overview

This project demonstrates how to fine-tune OpenAI's GPT-2 language model on the TinyStories dataset using the Hugging Face Transformers library.

The objective is to train a pretrained GPT-2 model to generate coherent and contextually relevant text. The notebook covers dataset preprocessing, model fine-tuning, evaluation, and text generation using different decoding strategies.

---

## Features

- Fine-tune GPT-2 on a custom text dataset
- Tokenization and preprocessing
- Training using Hugging Face Trainer API
- Model evaluation using Perplexity
- Text generation using:
  - Greedy Search
  - Beam Search
  - Top-k Sampling
  - Top-p (Nucleus) Sampling
- Save and reload fine-tuned models

---

## Dataset

Dataset Used:

**TinyStories**

The notebook uses a subset of approximately:

- 4000 training examples
- 400 validation examples

---

## Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- Accelerate
- Evaluate
- Google Colab

---

## Project Workflow

1. Load TinyStories Dataset
2. Tokenize Text
3. Group Tokens into Fixed-Length Sequences
4. Load Pretrained GPT-2
5. Fine-tune GPT-2
6. Save Model
7. Generate Text
8. Evaluate Model
9. Compare Decoding Strategies

---

## Model Configuration

| Parameter | Value |
|-----------|--------|
| Model | GPT-2 |
| Epochs | 3 |
| Block Size | 256 |
| Batch Size | 8 |
| Learning Rate | 5e-5 |

---

## Results

Training completed successfully.

Training Summary:

- Epochs: **3**
- Training Loss: **1.964**
- Evaluation Loss: **1.855**
- Perplexity: **6.39**

The fine-tuned model generated more coherent and contextually relevant stories than the base GPT-2 model.

---

## Sample Output

### Prompt

```
Once upon a time
```

### Generated Text

```
Once upon a time, there was a little girl named Lily who loved exploring the forest. One sunny morning she found a tiny bird that had fallen from its nest. Lily gently picked it up and searched for the tree where it belonged. With patience and kindness, she returned the bird safely to its family and happily walked home.
```

---

## Repository Structure

```
GPT2_Text_Generation.ipynb
README.md
requirements.txt
outputs/
images/
```

---

## Installation

```bash
git clone https://github.com/<your-username>/gpt2-text-generation.git

cd gpt2-text-generation

pip install -r requirements.txt
```

---

## Run

Open

```
GPT2_Text_Generation.ipynb
```

using Google Colab or VS Code Jupyter.

Run all cells sequentially.

---

## Learning Outcomes

This project demonstrates:

- Transformer-based Language Models
- GPT-2 Fine-Tuning
- Hugging Face Trainer API
- Tokenization
- Text Generation
- Language Model Evaluation
- Different Decoding Algorithms

---


