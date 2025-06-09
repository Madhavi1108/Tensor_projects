# Brain Tumor Detection Using Deep Learning

This project aims to detect brain tumors in MRI images using a Convolutional Neural Network (CNN) model implemented in Python with TensorFlow/Keras. The model is trained to classify brain MRI images into two categories: **Tumor** and **No Tumor**.

## 🧠 Project Overview

Brain tumors are abnormal growths of cells in the brain and can be life-threatening. Early detection through medical imaging, especially MRI, is crucial. This project demonstrates how deep learning can aid radiologists by automatically classifying MRI images.

## 📁 Dataset

The dataset used consists of MRI images, categorized as:

* **Yes** – Images with brain tumors.
* **No** – Images without brain tumors.

The data is split into training and testing sets and preprocessed before being fed into the CNN model.

## 🔧 Features

* Image preprocessing and resizing
* Data augmentation
* Binary classification using CNN
* Accuracy and loss visualization
* Model evaluation on test data

## 🛠️ Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Google Colab or Jupyter Notebook

## 🚀 How to Run

1. Clone this repository or download the notebook.
2. Install dependencies:

   ```bash
   pip install tensorflow numpy matplotlib
   ```
3. Download and prepare the dataset in appropriate train/test folders.
4. Run the notebook `Brain_Tumor_detection_using_deep_leraning.ipynb`.

## 📈 Results

The model shows good accuracy in classifying MRI scans into tumor and non-tumor categories. Training and validation accuracy/loss plots are provided for performance evaluation.

## 📄 License

This project is for academic and learning purposes.
