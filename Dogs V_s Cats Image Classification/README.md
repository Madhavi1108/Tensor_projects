## 🐶🐱 Dogs vs Cats Image Classification

A binary image classification project that distinguishes between images of dogs and cats using Convolutional Neural Networks (CNN) in TensorFlow. Built and tested in Google Colab.

---

### 📂 Dataset

* Source: [Kaggle - Dogs vs Cats](https://www.kaggle.com/datasets/salader/dogs-vs-cats)
* Structure:

  ```
  /train
      /dog
      /cat
  /test
      /dog
      /cat
  ```
* Images are resized to `256x256`.

---

### 🧠 Model Architectures

#### 🔹 Option 1: Transfer Learning with MobileNetV2

* Uses pre-trained MobileNetV2 (ImageNet weights)
* Frozen convolutional base
* Fine-tuning with dense layers:

  * GlobalAveragePooling2D → Dense(128, ReLU) → Dropout → Dense(1, Sigmoid)
* Pros: Fast convergence, high accuracy
* Cons: Larger size, more memory

#### 🔹 Option 2: Lightweight Custom CNN

* 3 convolutional layers with max pooling
* Flatten → Dense(128, ReLU) → Dropout → Dense(1, Sigmoid)
* Pros: Simpler, faster to train
* Cons: Slightly lower accuracy on small datasets

---

### 🧪 Preprocessing Steps

* Normalized pixel values to range \[0, 1]
* Applied image augmentation (flip, rotate, zoom) for generalization
* Batched datasets using `image_dataset_from_directory()`

---

### 🏁 Training

* Optimizer: `Adam`
* Loss: `Binary Crossentropy`
* Metrics: `Accuracy`
* Callbacks:

  * EarlyStopping (with patience = 3)
  * ModelCheckpoint (best model saved as `best_model.h5`)

---

### 📈 Evaluation

* Accuracy and loss plotted across epochs
* Confusion matrix + classification report generated
* Metrics include Precision, Recall, F1-Score

---

### 🧰 Technologies Used

* Python 3.x
* TensorFlow / Keras
* Matplotlib & Seaborn
* scikit-learn
* Google Colab
* Kaggle API

---

### ✅ How to Run

1. Upload your `kaggle.json` in Colab and set up Kaggle API.
2. Run the notebook (`Dogs_vs_cats_image_classification.ipynb`).
3. Choose between MobileNetV2 or custom CNN (both models available).
4. Evaluate and visualize results.

---

### 📌 Future Improvements

* Hyperparameter tuning (batch size, dropout rate)
* Add learning rate scheduler
* Try other architectures like EfficientNet or ResNet
* Use Grad-CAM to visualize attention maps

---

### 📸 Sample Results

* Accuracy: \~90% with MobileNetV2, \~85% with custom CNN
* Precision and recall balanced across both classes

