# MNIST Handwritten Digit Classifier

A Machine Learning project to recognize handwritten digits (0–9) using the famous MNIST dataset.

---

##  Project Overview

- **Objective:**  
  Train a deep learning model to classify handwritten digit images into classes 0–9.

- **Dataset:**  
  MNIST dataset consisting of 60,000 training images and 10,000 test images of handwritten digits.

- **Tech Stack:**  
  - Python
  - TensorFlow / Keras
  - Matplotlib / Seaborn
  - NumPy
  - Streamlit (for UI app)

---

## Features

- Preprocessing and normalization of MNIST images
- Convolutional Neural Network (CNN) model training
- Model evaluation using accuracy and loss curves
- Interactive Streamlit app:
  - Draw a digit on a canvas
  - Model predicts the digit in real-time
- Visualization of pixel-wise variance across the dataset
- Visual analytics like:
  - Label distribution
  - Average digit visualization
  - Heatmaps of pixel importance

---

##  How to Run

1. **Install dependencies:**
   ```bash
   pip install tensorflow numpy matplotlib seaborn streamlit streamlit-drawable-canvas opencv-python
   ```

2. **Train the model:**
   - Run the notebook `Mnsit_digit_classifier.ipynb`
   - Model is saved as `mnist_digit_model.h5`

3. **Run the Streamlit app:**
   ```bash
   streamlit run main.py
   ```
   This will open a browser window where you can draw a digit and check the prediction.

---

## Evaluation Metrics

- **Training Accuracy**
- **Validation Accuracy**
- **Training Loss**
- **Validation Loss**
- **Confusion Matrix** (optional if added)
- **Visualizations of Variance in Digit Pixels**

---

## Improvements Planned

- Training with data augmentation (rotation, shifting digits)
- Using deeper CNN architectures for even higher accuracy
- Adding a confidence score bar to Streamlit app
- Extending to multi-digit recognition

---

##  Contributions

Pull requests and suggestions are welcome!  
Feel free to fork and improve the model, UI, or analytics part of the project.

---

##  License

This project is open source and available under the [MIT License](LICENSE).

---

#  Summary
This project demonstrates how deep learning models can classify handwritten digits with high accuracy and how to build an interactive user-friendly digit recognition app.
