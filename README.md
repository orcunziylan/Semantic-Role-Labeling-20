# Semantic Role Labeling 2020

This repository contains the code and related files for the Natural Language Processing (NLP) Homework 2.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model](#model)
- [Training](#training)
- [Evaluation](#evaluation)

## Introduction

This project is part of the NLP course's Homework 2. It involves building and training a neural network model for semantic role labeling (SRL). The task aims to identify the predicate-argument structure in sentences, assigning roles to words in relation to a predicate.

## Dataset

The project uses the dataset provided in JSON format. It contains information about words, lemmas, part-of-speech tags, dependency heads, dependency relations, predicates, and roles. The dataset is split into training, development, and test sets.

## Model

The neural network model is implemented using PyTorch. The architecture includes an embedding layer, a Bi-LSTM layer, a dropout layer, and a linear classifier. Pre-trained GloVe embeddings are used as word representations. The model is designed to perform argument identification and argument classification.

## Training

The model is trained using the training dataset and optimized with the Adam optimizer. The loss is calculated using the CrossEntropyLoss function. Training progress is monitored, and the model's performance is evaluated on the validation dataset.

## Evaluation

The model's performance is evaluated on the test dataset. Two main evaluation metrics are used: argument identification F1-score and argument classification F1-score. These metrics provide insights into the model's ability to correctly identify and classify arguments in sentences.
