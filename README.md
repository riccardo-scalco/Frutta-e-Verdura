# Fruitify: AI-Powered Fruit & Vegetable Recognition

**Fruitify** is an Android application developed to explore the practical implementation of Image Classification using **TensorFlow**. The core of the app is a deep learning model trained to recognize various types of fruits and vegetables in real-time.

## 👥 Authors
* **Riccardo Scalco** 
* **Geremia Paoletto**
* **Lorenzo Berlese** 

## 🚀 Overview
The application leverages mobile computer vision to identify produce via the camera, providing nutritional information and allowing users to manage personalized grocery or pantry lists. It was developed to test image classification capabilities on mobile devices.

## 🛠️ Technical Stack
* **Deep Learning Framework**: TensorFlow / Keras.
* **Model Architecture**: MobileNetV2 (via Transfer Learning).
* **Mobile Platform**: Android (Tested on Android 12+).
* **Database**: Room (for local data persistence).
* **Training Environment**: Google Colab using GPU acceleration.

## 🧠 Model Development Pipeline
The model was custom-built following a structured data science workflow:
1.  **Data Acquisition**: Images were sourced and downloaded using the **Kaggle API**.
2.  **Preprocessing & Training**: A Python script was developed to process data and train the model using **MobileNetV2** as a backbone.
3.  **Optimization**: The training phase was executed on Google Colab to leverage high-performance cloud GPUs.

> **Note on Accuracy**: The model is trained on a limited dataset and epochs due to hardware constraints. Future improvements could involve dataset expansion and fine-tuning hyper-parameters.

## ✨ Key Features

### 1. Real-Time Recognition (AI Integration)
* **Dynamic Inference**: The app processes a bitmap buffer from the camera feed for periodic predictions.
* **Confidence Threshold**: Results are only displayed if the model's confidence exceeds a **90% threshold**.
* **Direct Action**: Recognized items can be added to lists or used to view nutritional data immediately.

### 2. Intelligent List Management
* **CRUD Operations**: Users can create, rename (via AndroidX Dialogs), and delete multiple lists.
* **Database Integrity**: Lists are uniquely identified by a numerical ID in the **Room database**.
* **Smart Quantity Handling**: Adding an existing item automatically increments its quantity.

### 3. Nutritional Database
* **Search Functionality**: A manual search allows users to find specific fruits or vegetables.
* **Detailed Insights**: Nutritional values are provided for every supported produce type.

## 📸 Permissions & Requirements
* **Camera Access**: Essential for the real-time recognition feature.
* **OS Compatibility**: Primarily tested on Android 12, but compatible with newer versions.

---
*Icons and visual assets sourced from Flat Icon, Freepik, and Pexels.*
