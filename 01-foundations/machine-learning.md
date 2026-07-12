# Machine Learning Basics

## Overview

Machine Learning (ML) is a branch of Artificial Intelligence that enables computers to learn patterns from data without being explicitly programmed for every task.

Instead of manually writing rules, ML algorithms identify relationships within data and use those relationships to make predictions or decisions.

---

# Why Machine Learning?

Traditional Programming

Input + Rules
        |
        v
     Output

Machine Learning

Input + Output
        |
        v
   Learning Algorithm
        |
        v
      Model

---

# Types of Machine Learning

## 1. Supervised Learning

Definition

Learning from labeled data.

Example

Email Spam Detection

Input

Email

Output

Spam / Not Spam

Algorithms

- Linear Regression
- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine
- Neural Networks

Applications

- Image Classification
- Fraud Detection
- Medical Diagnosis

---

## 2. Unsupervised Learning

Definition

Learning hidden patterns from unlabeled data.

Algorithms

- K-Means
- DBSCAN
- Hierarchical Clustering

Applications

- Customer Segmentation
- Topic Modeling
- Recommendation Systems

---

## 3. Reinforcement Learning

Definition

Learning through rewards and penalties.

Components

- Agent
- Environment
- Action
- Reward

Applications

- Robotics
- Game AI
- Autonomous Driving

---

# Machine Learning Workflow

Problem Definition

↓

Collect Data

↓

Clean Data

↓

Feature Engineering

↓

Train Model

↓

Evaluate Model

↓

Deploy Model

↓

Monitor Performance

---

# Dataset

A dataset consists of:

- Features (Input)
- Labels (Output)

Example

| Hours Studied | Exam Result |
|--------------|-------------|
| 2 | Fail |
| 5 | Pass |
| 8 | Pass |

---

# Features

Features are input variables.

Example

House Price Prediction

Features

- Area
- Bedrooms
- Bathrooms
- Location

Target

House Price

---

# Training vs Testing

Training Set

Used for learning.

Testing Set

Used for evaluation.

Typical Split

80% Training

20% Testing

---

# Model

A machine learning model learns relationships from data.

Goal

Find a function:

Input → Output

---

# Loss Function

Measures prediction error.

Lower Loss

↓

Better Model

Common Loss Functions

- Mean Squared Error
- Cross Entropy Loss

---

# Optimization

Most ML models use Gradient Descent.

Workflow

Prediction

↓

Loss

↓

Gradient

↓

Update Parameters

↓

Repeat

---

# Evaluation Metrics

Classification

- Accuracy
- Precision
- Recall
- F1 Score

Regression

- MAE
- MSE
- RMSE
- R² Score

---

# Overfitting

Model memorizes training data.

Problem

Poor generalization.

Solutions

- More data
- Regularization
- Dropout
- Early Stopping

---

# Underfitting

Model is too simple.

Problem

Cannot learn patterns.

Solutions

- Better model
- More features
- Longer training

---

# Bias-Variance Tradeoff

High Bias

↓

Underfitting

High Variance

↓

Overfitting

Goal

Balanced Model

---

# Common ML Algorithms

Regression

- Linear Regression

Classification

- Logistic Regression
- SVM
- Decision Tree
- Random Forest

Clustering

- K-Means

Dimensionality Reduction

- PCA

Deep Learning

- Neural Networks

---

# Applications

Healthcare

Finance

Cybersecurity

Natural Language Processing

Computer Vision

Software Engineering

Recommendation Systems

---

# Machine Learning vs Deep Learning

Machine Learning

- Feature Engineering Required
- Smaller Data
- Faster Training

Deep Learning

- Learns Features Automatically
- Large Dataset
- Higher Accuracy

---

# Relation to Large Language Models

LLMs are built using Deep Learning.

Pipeline

Machine Learning

↓

Deep Learning

↓

Transformers

↓

Large Language Models

↓

AI Agents

↓

RAG Systems

---

# Relation to My Research

This foundation supports my research in:

- Retrieval-Augmented Generation
- AI Software Engineering
- Intelligent Code Generation
- AI Coding Agents
- Autonomous Software Engineering

---

# Summary

Machine Learning provides the theoretical foundation for modern AI systems. Understanding supervised learning, unsupervised learning, optimization, evaluation, and model generalization is essential before studying Deep Learning, Transformers, Large Language Models, Retrieval-Augmented Generation, and AI Agents.
