# 🌤️ Weather Image Classification (PyTorch)

End-to-end CNN model built in PyTorch to classify weather images into 11 categories.

---

## 📊 Dataset & Setup

* **Dataset:** 6,862 images across 11 classes (`dew`, `fogsmog`, `frost`, `glaze`, `hail`, `lightning`, `rain`, `rainbow`, `rime`, `sandstorm`, `snow`).
* **Split:** 70% Train (4,803), 15% Val (1,029), 15% Test (1,030).
* **Preprocessing:** Standardized to $128 \times 128 \times 3$, normalized (ImageNet stats), with data augmentations (flip, rotation, color jitter) on training data.

---

## 🏗️ Model Architecture

Custom 3-layer Convolutional Neural Network (`WeatherCNN`):
* **Features:** 3× Conv2D (32, 64, 128 channels) + ReLU + MaxPool2D.
* **Classifier:** Flatten $\rightarrow$ Linear(32768, 128) $\rightarrow$ ReLU $\rightarrow$ Dropout(0.5) $\rightarrow$ Linear(128, 11).
* **Setup:** Adam ($\text{lr}=0.001$), `CrossEntropyLoss`, Early Stopping ($\text{patience}=3$).

---

## 📈 Results

* **Test Loss:** `0.7963`
* **Test Accuracy:** **`73.88%`**

### Key Takeaways
* **Best Classes:** `lightning` (>91% accuracy) and `rime` (141 correct predictions).
* **Main Confusion:** High feature overlap between `frost` and `glaze`.
* **Imbalance Bias:** `rime` absorbs false positives due to its large sample size.