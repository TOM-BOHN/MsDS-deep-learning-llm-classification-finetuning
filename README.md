# LLM Classification Finetuning: Predicting Human Preferences

This repository contains the code and documentation for a project focused on predicting human preferences in Large Language Model (LLM) responses. The project uses the Chatbot Arena dataset to train and evaluate a DeBERTa v3 model for this classification task.

## Executive Summary

This project presents a systematic approach to developing machine learning models for predicting human preferences in large language model (LLM) responses, addressing the critical challenge of aligning AI systems with human values and preferences. The work implements a comprehensive experimental framework using the Chatbot Arena dataset, containing 57,477 training examples of human-AI interactions with preference judgments across three classes: model A wins, model B wins, or tie. The methodology focuses on three key phases: baseline establishment using a DeBERTa v3 extra-small model, code modernization with modular functions, and systematic experimental optimization through three distinct experiments. The systematic approach aligns with measurable improvements in accuracy, F1-score, and log loss while maintaining computational efficiency, ultimately providing insights into which methodologies work best for this challenging classification task and demonstrating practical implementation strategies for handling large-scale text classification problems.

## Key Results and Findings

The project demonstrates a systematic improvement in model performance across three experiments.

* **Experiment 1 - Optimizer Enhancement**: This experiment enhanced the baseline with the AdamW optimizer and weight decay regularization to reduce overfitting and improve generalization.
* **Experiment 2 - Extended Context**: This experiment upgraded to a larger DeBERTa v3 small model with an extended context of 1024 tokens versus the baseline's 512 tokens.
* **Experiment 3 - Enhanced Architecture**: This experiment implemented a multi-layer classification head with dropout regularization for more sophisticated decision-making capabilities.

Each experiment targeted and achieved improvements in accuracy, F1-score, and log loss, demonstrating the effectiveness of the systematic optimization approach.

## Model Used

The core model used in this project is the **DeBERTa v3 (Decoding-enhanced BERT with disentangled attention)**.

The project started with a **DeBERTa v3 extra-small** model as a baseline and then experimented with a larger **DeBERTa v3 small** model. The DeBERTa v3 model was chosen for its state-of-the-art performance on a wide range of NLP tasks. The model architecture was further enhanced by implementing a multi-layer classification head with dropout regularization in Experiment 3. The project utilizes the `keras_nlp` library for implementing the DeBERTa v3 model and its preprocessor.
