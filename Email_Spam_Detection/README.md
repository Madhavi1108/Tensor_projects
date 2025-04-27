# Email Spam Detection Project

A Machine Learning project to classify emails as **Spam** or **Not Spam** using deep learning (LSTM / Neural Network).

---

## Project Overview

- **Objective:**  
  Build a model that can automatically detect if an email is spam or not based on its text content.

- **Dataset:**  
  Preprocessed email texts labeled as "spam" or "ham" (not spam).

- **Tech Stack:**  
  - Python
  - TensorFlow / Keras
  - Scikit-learn
  - Natural Language Processing (NLP)
  - Matplotlib / Seaborn (for visualization)

---

## Features

- Tokenization and sequence padding of email text
- Deep Learning model training (with EarlyStopping & ReduceLROnPlateau)
- Real-time **Email Prediction Function**:
  - Takes a text input and predicts Spam or Not Spam
  - Shows prediction confidence
- Visualization of training accuracy and loss curves
- Evaluation metrics (classification report, confusion matrix)

---

## How to Run

1. **Install dependencies:**
   ```bash
   pip install tensorflow scikit-learn matplotlib seaborn
   ```

2. **Run the notebook `Email_Spam_Detection.ipynb`**:
   - It preprocesses the text.
   - Trains the spam detection model.
   - Evaluates and visualizes performance.
   - Provides a `predict_email(text)` function for real-time testing.

3. **Example usage:**

   ```python
   email_text = "Congratulations! You've won a $1000 Walmart gift card."
   print(predict_email(email_text))
   ```

---

## Evaluation Metrics

- **Accuracy** on test set
- **Classification Report** (Precision, Recall, F1-Score)
- **Confusion Matrix** to visualize model predictions

---

## Improvements Planned

- Better text cleaning (removal of stopwords, lemmatization)
- Training on larger, real-world email datasets
- Threshold tuning using ROC Curve
- Streamlit Web App interface (future plan)

---

## Contributions

Pull requests and suggestions are welcome!  
Feel free to fork the repo and improve the spam detection pipeline.

---

## License

This project is open source and available under the [MIT License](LICENSE).

---

# Summary
This project demonstrates how deep learning models can be used for text classification tasks like email spam detection, with real-time prediction capabilities!

---
