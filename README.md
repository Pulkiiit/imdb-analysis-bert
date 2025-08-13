# 🎬 IMDb Sentiment Classification with Transformers

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/191eUE2hSgudijPSuD-NvCR23Ocznu5dj?usp=sharing)
[![W&B Report](https://img.shields.io/badge/Weights_&_Biases-View%20Report-orange?logo=weightsandbiases)]([YOUR_REPORT_LINK](https://api.wandb.ai/links/pulkiiit-infosys/d76a8m8m))

This project fine-tunes a pretrained Transformer (e.g., `distilbert-base-uncased`) on the IMDb movie reviews dataset to perform binary sentiment classification (positive or negative). It demonstrates transfer learning for NLP using the Hugging Face `transformers` library and PyTorch.

---

## 🚀 Features

- ✅ Fine-tunes a Transformer on the IMDb reviews dataset
- 🧠 Uses a custom PyTorch `Dataset` wrapper
- 🔁 Automatic padding with `DataCollatorWithPadding`
- 📊 Tracks accuracy, precision, recall, and F1 score
- 📈 Plots training and validation loss
- 💾 Saves the fine-tuned model and tokenizer

---

## 📚 Dataset

- Source: [`keras.datasets.imdb`](https://www.tensorflow.org/api_docs/python/tf/keras/datasets/imdb)
- 50,000 labeled movie reviews (25,000 train / 25,000 test)
- Binary sentiment labels: 0 (negative), 1 (positive)

---

## 🧠 Model & Training Details

- **Model**: `distilbert-base-uncased`
- **Tokenizer**: Hugging Face tokenizer with truncation and dynamic padding
- **Epochs**: 4
- **Batch Size**: 16
- **Max Sequence Length**: 512

---

## 🧪 Evaluation Metrics

Achieved the following on the IMDb test set:

Accuracy : 93.02%
Precision : 93.03%
Recall : 93.01%
F1 Score : 93.02%

---
