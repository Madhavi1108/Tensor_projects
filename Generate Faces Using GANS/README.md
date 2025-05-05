# 🎭 Generate Faces Using GANs

This project demonstrates how to **generate human-like faces** using **Generative Adversarial Networks (GANs)**. Built from scratch using TensorFlow and trained on a custom dataset, this GAN learns to synthesize realistic facial images through an adversarial process between a generator and discriminator.

---

## 🧠 About the Model

A **Deep Convolutional GAN (DCGAN)** is implemented with:

* **Generator**: Takes a random noise vector and outputs a synthetic face image.
* **Discriminator**: Judges whether the image is real or generated.
* **Adversarial Training**: The generator improves by learning to fool the discriminator, while the discriminator improves by distinguishing real from fake.

> This is based on the original DCGAN architecture described in [Radford et al., 2015](https://arxiv.org/abs/1511.06434).

---

## 📂 Project Structure

```
├── Genrate_faces_using_GANS.ipynb   # Complete implementation in Jupyter Notebook
├── images/                          # Folder containing generated face images per epoch
│   ├── epoch_0.png
│   ├── epoch_100.png
│   └── ...
└── README.md                        # Project documentation
```

---

## 🛠️ Tech Stack

* **Language**: Python
* **Framework**: TensorFlow (Keras API)
* **Visualization**: Matplotlib
* **Environment**: Google Colab / Jupyter Notebook

---

## 🧪 How It Works

1. **Input**: A 100-dimensional random noise vector.
2. **Generation**: Generator transforms the noise into a fake face image.
3. **Classification**: Discriminator evaluates images as "real" or "fake".
4. **Training Loop**: Both networks improve through adversarial learning.
5. **Output**: Faces are generated and saved at every epoch using:

```python
generate_and_save_images(generator, epoch, test_input)
```

Images are saved to the `images/` directory for visualization.

---
## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Generate-faces-using-GANs.git
cd Generate-faces-using-GANs
```

### 2. Open the Notebook

* Use **Google Colab** or **Jupyter Notebook** to open `Genrate_faces_using_GANS.ipynb`.

### 3. Run All Cells

* Ensure the required libraries are installed (`tensorflow`, `matplotlib`, `numpy`)
* The model will train and generate output images at regular intervals

---

## 💡 Notes

* The training uses a small sample dataset. For better results, use high-quality datasets like **CelebA**.
* Training GANs requires GPU for performance — recommended to use **Colab GPU runtime**.
* The generated face images start off as noisy blobs and gradually become human-like.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

