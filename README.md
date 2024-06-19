<h1 align="center">Dermafie Machine Learning</h1>

<div align="center">

![Python](https://img.shields.io/badge/-Python-05122A?style=flat&logo=python)&nbsp;
![TensorFlow](https://img.shields.io/badge/-TensorFlow-05122A?style=flat&logo=tensorflow)&nbsp;
![NumPy](https://img.shields.io/badge/-NumPy-05122A?style=flat&logo=numpy)&nbsp;
![Matplotlib](https://img.shields.io/badge/-Matplotlib-05122A?style=flat&logo=matplotlib)&nbsp;
![Google Colab](https://img.shields.io/badge/-Google%20Colab-05122A?style=flat&logo=googlecolab)&nbsp;

</div>

# Dermafie Machine Learning

## Table of Contents

- [Introduction](#introduction)
- [Folder Structure](#folder-structure)
- [Prerequisites](#prerequisites)
- [Architectures](#architectures)
- [Dataset](#dataset)
- [Setup](#setup)

## Introduction
- This repository contains two machine learning models that have been trained to do classification tasks and object detection tasks.
- The classification model is trained to classify **four classes** of skin conditions, which are healthy, rosacea, basal cell, and melanoma. The model has also been converted into a TensorflowJS model that is ready to use.
- The object detection model is trained to be able to detect **nine classes** of skin conditions, which are rosacea, basal cell, melanoma, dark spots, blackheads, nodules, pustules, papules, and whiteheads. as of tensorflowjs version 4.20.0, there are some Unsupported Ops in the model and currently TensorFlow.js only supports a limited set of TensorFlow Ops. But the TFLite model can be used instead.

## Folder Structure
- **Classification Model**: Direktori ini berisi notebook yang dapat dijalankan di Google Colab untuk membangun dan melatih model klasifikasi.
- **Object Detection Model**: Direktori ini terdapat model object detection yang dibangun untuk mendetek 9 kelas penyakit

## Architectures
Each task of the model used the following architecture:
* Classification used InceptionV3 architecture pretrained with imagenet
* Object Detection used Retinanet model with ResNet-50 as the backbone and FPN (Feature Pyramid Network) for the decoder

## Prerequisites
- Python version 3.10 or later
- The Python packages listed in the requirements.txt

## Dataset
- For Classification use this [dataset](https://app.roboflow.com/dermafie/dermafie-classification)
- For Object detection use this [dataset](https://app.roboflow.com/dermafie/dermafie)

## Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Dermafie/dermafie-ml.git
   ```
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```