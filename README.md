# MediParse: Multi-Label Sentence Classification for Medical Texts

**MediParse** is a multi-label sentence classification project designed for medical research abstracts, leveraging a tribrid embedding model to accurately categorize sentences from the PubMed RCT dataset. The project implements various NLP techniques, achieving high accuracy in sentence classification by combining token, character, and positional embeddings.

## Project Overview

In this project, six different NLP models were explored to classify sentences in the PubMed RCT dataset. Through a progression of techniques—from TF-IDF to hybrid embeddings—the final **Model_5 (tribrid model)** demonstrated superior performance across all evaluation metrics, achieving an accuracy, precision, recall, and F1-score of 83.33%.

## Key Features

- **Multi-label Classification**: Classifies each sentence with multiple relevant labels, capturing complex sentence roles in medical abstracts.
- **Advanced Embedding Techniques**: Combines token, character, and positional embeddings to create a robust representation for nuanced classification.
- **High Performance**: Achieves 83.33% across accuracy, precision, recall, and F1-score with the tribrid model.

## Dataset

The project uses the [PubMed RCT](https://github.com/Franck-Dernoncourt/pubmed-rct) dataset, a collection of medical research abstracts labeled with key components like objectives, methods, and results.

## Model Overview

| Model Name   | Description                                                |
|--------------|------------------------------------------------------------|
| Baseline     | Uses TF-IDF vectorization.                                 |
| Model_1      | Employs custom token embeddings.                           |
| Model_2      | Utilizes pretrained token embeddings.                      |
| Model_3      | Implements character embeddings.                           |
| Model_4      | Combines token and character embeddings.                   |
| **Model_5**  | **Tribrid Model**: Integrates token, character, and positional embeddings, achieving the highest performance. |

## Results

| Model      | Accuracy | Precision | Recall | F1 Score |
|------------|----------|-----------|--------|----------|
| Baseline   | **72.18%** | **0.71** | **0.72** | **0.69** |
| Model_1    | **78.34%** | **0.78** | **0.78** | **0.78** |
| Model_2    | **71.59%** | **0.71** | **0.71** | **0.72** |
| Model_3    | **66.00%** | **0.65** | **0.66** | **0.64** |
| Model_4    | **73.42%** | **0.73** | **0.73** | **0.73** |
| **Model_5**| **83.33%** | **0.83** | **0.83** | **0.83** |

*Model_5 achieved the highest performance in all metrics, making it the optimal choice for this multi-label classification task.*
