**Financial Sentiment Fine-Tuning**

This project evaluates two fine-tuning strategies — Full Fine-Tuning and Low-Rank Adaptation (LoRA) — for adapting pretrained Transformer models to financial sentiment analysis.
All experiments can be reproduced using the provided notebook and dataset.

**1. Files in This Repository**
notebook.ipynb	Main Jupyter Notebook for preprocessing, fine-tuning, evaluation, and visualization
READ.me Instructions

**2. Installation**

**Clone this repository**

**Install required libraries**

The project was tested with the following package versions:

Library	Version:
transformers	4.37.2
datasets	2.16.1
torch	2.9.0
peft	0.10.0
evaluate	0.4.0

To install all dependencies:

pip install transformers==4.37.2 datasets==2.16.1 torch==2.9.0 peft==0.10.0 evaluate==0.4.0



**Dataset Preparation**

The dataset merges FiQA and Financial PhraseBank data from Kaggle, providing labeled financial sentences for sentiment classification:
Download the data from kaggle: https://www.kaggle.com/datasets/sbhatti/financial-sentiment-analysis?resource=download
and rename it as financial.csv


Columns: Sentence, Sentiment

Labels: positive, neutral, negative

No additional preprocessing is required — the notebook automatically loads and encodes labels.

**Running the Experiments**
Step 1. Launch Jupyter Notebook
jupyter notebook notebook.ipynb

Step 2. Run All Cells
Each cell includes progress printouts and checkpoints to verify that each step runs correctly.
