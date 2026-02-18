# Alfaisal Postdoctoral Technical Challenge
Medical Image Analysis – PneumoniaMNIST
This repository contains my submission for the 7-Day Postdoctoral Technical Challenge at AlfaisalX – Cognitive Robotics and Autonomous Agents, MedX Research Unit.

# Overview

This project implements a complete end-to-end AI pipeline for medical imaging, including:

- CNN-based pneumonia classification
- Automated medical report generation
- Semantic image retrieval system

All experiments were conducted using the PneumoniaMNIST dataset from MedMNIST v2.

# Task 1 – CNN Classification


Model: ResNet18  
Dataset: PneumoniaMNIST  
Input size: 224×224  
Loss function: CrossEntropyLoss  
Optimizer: Adam  

The model was fine-tuned for binary classification (Normal vs Pneumonia).  
The trained weights are saved as:

best_model.pth


# Task 2 – Medical Report Generation

A structured medical-style report is generated based on the predicted class.

- If Normal → report indicates absence of infection.
- If Pneumonia → report describes radiographic signs consistent with pneumonia.

This demonstrates integration of visual AI into clinical-style reporting systems.

# Task 3 – Semantic Image Retrieval

The trained ResNet18 was used as a feature extractor.

Embedding size: 512  
Normalization: L2  
Similarity search: FAISS (Inner Product)

Evaluation metric: Precision@5  

Result:

Precision@5 = 0.90

This demonstrates strong clustering of pathology-specific patterns.

# Repository Structure

- Task1_CNN_PneumoniaMNIST.ipynb
- Task2_Report_Generation.ipynb
- Task3_Image_Retrieval.ipynb
- best_model.pth
- Medical_Image_Analysis_Challenge_Report.docx


# Author

dr.Kaouther SELMI
