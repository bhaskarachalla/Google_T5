# Google T5 Fine-Tuning

This repository contains code and resources for fine-tuning the T5 (Text-to-Text Transfer Transformer) model on custom datasets, specifically tailored for question-answering tasks. The model is based on the pre-trained T5 architecture developed by Google.

## Table of Contents

- Introduction
- Requirements
- Dataset Preparation
- Training the Model
- Inference
- License

## Introduction

The T5 model reframes all NLP tasks into a unified text-to-text format. This approach allows for versatile applications, including text generation, translation, summarization, and question answering. This repository provides a step-by-step guide to fine-tune the T5 model on your own dataset.

## Requirements

To run the code, you will need:

- Python 3.6 or later
- PyTorch
- Transformers library from Hugging Face
- GPU if possible.

## Dataset Preparation

Prepare your dataset in a CSV format with at least two columns: `question` and `answer`. The dataset should contain pairs of questions and their corresponding answers.

## Training the Model

To train the model, run the training script provided in the repository. The script will handle data loading, preprocessing, and model training. Ensure that your environment is set up to utilize GPU if available, or it will default to CPU.

### Training Arguments

You can modify training parameters such as learning rate, batch size, and number of epochs directly in the training script. The default settings should work for most cases but can be adjusted for your specific dataset.

## Inference

After training, you can test the model with your own questions. The inference script will load the trained model and return the predicted answer based on the question you provide.
