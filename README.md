# Plant Infection Detection System

## Table of Contents
- [Introduction](#1-introduction)
  - [Project Overview](#11-project-overview)
  - [Scope](#12-scope)
  - [Objective](#13-objective)
- [System Analysis](#2-system-analysis)
  - [Tools and Technology](#21-tools-and-technology)
  - [Project Category](#22-project-category)
- [Implementation](#3-implementation)
  - [Implementation Strategy](#31-implementation-strategy)
  - [Steps to Execute](#32-steps-to-execute)
  - [Dataset Creation](#33-dataset-creation)
  - [Model Building](#34-model-building)
- [Constraints and Future Enhancement](#4-constraints-and-future-enhancement)
  - [Constraints](#41-constraints)
  - [Future Enhancement](#42-future-enhancement)
- [Project Documents](#5-project-documents)


## 1. Introduction

### 1.1 Project Overview

Plant diseases are a common issue in agriculture that can have significant negative effects on crop quality and productivity. This project focuses on the automatic detection of plant diseases using machine learning and image processing techniques. Early disease detection is crucial to prevent large-scale outbreaks and minimize the impact on crops.

### 1.2 Scope

The scope of this project is to develop a machine learning and image processing-based application that can detect diseases in plant leaves uploaded by users. The application aims to assist farmers and researchers in quickly identifying leaf diseases, which can lead to timely actions and the production of bio products based on the identified diseases.

### 1.3 Objective

The main objective of this project is to analyze and identify leaf diseases using image processing and machine learning. The project aims to help farmers and researchers by providing accurate disease detection, which can improve the quality and productivity of agricultural products.

## 2. System Analysis

### 2.1 Tools and Technology

#### Software Requirement

- Python
- OpenCV library
- Scikit learn library (SVM)
- SKlearn
- Numpy
- Mathlib Library

#### Project Category

Machine Learning

## 3. Implementation

### 3.1 Implementation Strategy

The implementation strategy includes several steps:

1. RGB image acquisition
2. Convert RGB to HSI format
3. Mask green pixels
4. Segment components
5. Extract useful segments
6. Evaluate feature parameters
7. Configure SVM for disease detection

### 3.2 Steps to Execute

Step 1: Run `GUIdriver.py` for image segmentation and feature extraction.
Step 2: Call `classifier.py` in `main.py` for classifying the leaf in the input image as "infected" or "healthy".

### 3.3 Dataset Creation

To create the dataset, run `leafdetectionALLsametype.py` for images of the same category (infected/healthy) and `leafdetectionALLmix.py` for a mixed dataset of both categories. The code runs on `.jpg`, `.jpeg`, and `.png` image formats in the specified directory.

### 3.4 Model Building

Support Vector Machine (SVM) is used as the classification model. Tuning parameters include Kernel, Regularization, Gamma, and Margin. SVM provides accurate classification by creating an optimal hyperplane that separates different classes.

## 4. Constraints and Future Enhancement

### 4.1 Constraints

- Low-resolution photos or improper lighting may lead to incorrect results.
- Certain leaf conditions, like a broken midrib, might result in false positives.

### 4.2 Future Enhancement

- Implementation on Raspberry Pi with PiCamera for live input.
- Exploring alternate methods to improve disease identification accuracy.
## 5. Project Documents

📂 **Explore Project Artifacts**: If you're curious about our project's journey, including presentation slides and comprehensive reports, take a stroll through our [Google Drive repository](https://drive.google.com/drive/u/1/folders/1P7llb1XD1o2473LPR3KrGepJBMcRhxPu).

🔍 **A Closer Look at Operation**: Delve deeper into the workings of our system! The report provides an immersive experience, guiding you through each step. You'll find an assortment of vibrant screenshots alongside step-by-step instructions, allowing you to witness the system's functionality firsthand.

Enjoy the journey of discovery and exploration! 🚀


