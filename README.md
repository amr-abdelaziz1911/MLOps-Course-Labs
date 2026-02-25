# 🚀 ML1 Project with MLflow Integration

## 📌 Project Overview

This repository extends the ML1 Machine Learning project by integrating
MLflow for experiment tracking, model comparison, and model registry
management.

The goal is to demonstrate clean ML workflows, reproducibility, and
structured MLOps practices.

------------------------------------------------------------------------

## 🎯 What Problem Does This Project Solve?

This project builds a complete machine learning pipeline for
classification tasks with full experiment tracking.

It focuses on:

-   Comparing multiple models
-   Tracking metrics and parameters
-   Registering and versioning models
-   Ensuring reproducibility

This makes it suitable for academic projects, ML experimentation, and
MLOps learning.

------------------------------------------------------------------------

## ⭐ Key Features

-   End-to-end ML pipeline
-   Data preprocessing and feature scaling
-   Multiple model training and comparison
-   Manual MLflow logging (no autolog)
-   Model Registry with versioning
-   Clean project structure
-   Reproducible environment setup

------------------------------------------------------------------------

## 🧠 Training Results Summary

The following models were evaluated:

  -----------------------------------------------------------------------
  Model           Accuracy            F1 Score            Notes
  --------------- ------------------- ------------------- ---------------
  Logistic        High baseline       Stable              Simple &
  Regression                                              interpretable

  Random Forest   Best performance    Strong F1           Selected final
                                                          model

  KNN             Moderate            Sensitive to        Secondary
                                      scaling             option
  -----------------------------------------------------------------------

### Key Observations

-   Random Forest achieved the strongest overall performance.
-   Logistic Regression provided a stable baseline.
-   MLflow enabled easy comparison between experiment runs.

------------------------------------------------------------------------

## ⚙️ System Pipeline

Pipeline steps:

1.  Load dataset
2.  Clean & preprocess data
3.  Split into train/test sets
4.  Apply feature scaling
5.  Train multiple models
6.  Evaluate metrics
7.  Log parameters & metrics to MLflow
8.  Register best-performing model

------------------------------------------------------------------------

## 📂 Project Structure

ML1-and-MLflow-project/

-   data/
-   notebooks/
-   src/
    -   train.py
    -   infer.py
    -   mlflow_utils.py
-   models/
-   requirements.txt
-   README.md

------------------------------------------------------------------------

## 🛠 How to Run This Project

### 1️⃣ Clone the repository

    git clone <your-repository-url>
    cd ML1-and-MLflow-project

### 2️⃣ Create environment

    conda create -n ml1_env python=3.10
    conda activate ml1_env

### 3️⃣ Install dependencies

    pip install -r requirements.txt

### 4️⃣ Train the model

    python src/train.py

### 5️⃣ Launch MLflow UI

    mlflow ui

Then open:

    http://127.0.0.1:5000

------------------------------------------------------------------------

## ⚡ Quick Test

To quickly verify everything works:

    python src/infer.py

------------------------------------------------------------------------

## 🧪 Experiment Tracking

All experiments are logged using MLflow.

Logged items:

-   Model parameters
-   Evaluation metrics
-   Artifacts (models, reports)
-   Model versions

Stored locally inside:

    mlruns/
