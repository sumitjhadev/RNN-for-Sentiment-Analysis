
<div align="center">

🧠 RNN SENTIMENT ANALYSIS

A Recurrent Neural Network built with PyTorch for binary text classification

<p>
  <img src="https://img.shields.io/badge/Python-3.11-3776AB?style=flat-square&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/PyTorch-RNN-EE4C2C?style=flat-square&logo=pytorch&logoColor=white">
  <img src="https://img.shields.io/badge/NLP-TF--IDF-8A2BE2?style=flat-square">
  <img src="https://img.shields.io/badge/Test%20Accuracy-85.16%25-2E8B57?style=flat-square">
</p>

From raw text → numerical representation → recurrent neural network → prediction

</div>

⚡ Project Overview

This project focuses on building and training a Recurrent Neural Network (RNN) from scratch using PyTorch for binary sentiment classification.

The main objective is to demonstrate the complete deep-learning workflow:

Preprocess → Vectorize → Prepare Tensors → Build RNN → Train → Evaluate

The model achieved a test accuracy of 85.16%.

🧩 Architecture

flowchart LR
    A["📝 Raw Text"] --> B["🧹 NLP Preprocessing"]
    B --> C["🔢 TF-IDF<br/>5,000 Features"]
    C --> D["🔥 PyTorch RNN"]
    D --> E["🧠 Hidden State<br/>128"]
    E --> F["📐 Linear Layer"]
    F --> G["🎯 Binary Prediction"]

🧠 The RNN

The core of this project is a PyTorch nn.RNN.

Model Configuration

Parameter

Value

Architecture

nn.RNN

Hidden Size

128

Input Features

5,000

Loss Function

BCELoss

Optimizer

Adam

Training Epochs

10

Output

Binary Classification

Test Accuracy

85.16%

🔄 Data → Model Flow

flowchart TD
    A["Dataset"] --> B["Clean Text"]
    B --> C["Lowercase"]
    C --> D["Remove URLs / HTML / Punctuation"]
    D --> E["Remove Stopwords"]
    E --> F["Porter Stemming"]
    F --> G["TF-IDF Vectorization"]
    G --> H["TensorDataset"]
    H --> I["DataLoader"]
    I --> J["PyTorch RNN"]
    J --> K["Binary Output"]

📊 Model Result

<div align="center">

🎯 85.16% Test Accuracy

</div>

xychart-beta
    title "RNN Test Accuracy"
    x-axis ["RNN"]
    y-axis "Accuracy (%)" 0 --> 100
    bar [85.16]

Final recorded test accuracy: 85.1568%

📈 Training Setup

flowchart LR
    A["10 Epochs"] --> B["RNN Training"]
    B --> C["Adam Optimizer"]
    C --> D["BCELoss"]
    D --> E["Evaluation"]

The training pipeline uses mini-batches through PyTorch DataLoader, followed by evaluation on the held-out test set.

🗂️ Project Structure

RNN-for-Sentiment-Analysis/
│
├── 📓 imdb-sentiment-analysis-rnn.ipynb
├── 📄 IMDB Dataset.csv
└── 📘 README.md

🛠️ Tech Stack

<div align="center">

Technology

Role

🐍 Python

Core programming

🔥 PyTorch

RNN & deep learning

🔤 NLTK

NLP preprocessing

📊 Scikit-learn

TF-IDF & data splitting

🐼 Pandas

Data handling

📓 Jupyter / Colab

Notebook development

</div>

🚀 Run The Project

1. Clone

git clone https://github.com/sumitjhadev/RNN-for-Sentiment-Analysis.git
cd RNN-for-Sentiment-Analysis

2. Install dependencies

pip install pandas nltk scikit-learn torch

3. Open the notebook

jupyter notebook

Open:

imdb-sentiment-analysis-rnn.ipynb

Then run the notebook cells from top to bottom.

✨ What This Project Demonstrates

🧠 Building an RNN with PyTorch

🔄 Preparing text data for neural networks

🔢 Converting text into numerical features with TF-IDF

🧹 Practical NLP preprocessing

⚙️ Training with Adam + BCELoss

📦 Working with PyTorch TensorDataset and DataLoader

📊 Evaluating a binary classification model

🎯 Achieving 85.16% test accuracy

🏁 Final Takeaway

This project is primarily a demonstration of how a Recurrent Neural Network can be implemented, trained, and evaluated using PyTorch.

The dataset provides the text classification task, but the central focus of the project is the RNN architecture and its complete training pipeline.

<div align="center">

🧠 BUILD • TRAIN • EVALUATE • LEARN

RNN Sentiment Analysis | PyTorch

⭐ If you like the project, consider giving it a star!

</div>
