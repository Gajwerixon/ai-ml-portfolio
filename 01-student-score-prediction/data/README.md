## 📊 Dataset

The dataset used in this project was obtained from Kaggle.

- **Dataset:** [Exam Score Prediction Dataset](https://www.kaggle.com/datasets/kundanbedmutha/exam-score-prediction-dataset)
- **Source:** Kaggle
- **License:** CC BY 4.0
- **Purpose:** Educational and portfolio demonstration

> **Note:** The raw dataset is not included directly in this GitHub repository to keep it lightweight. Instead, it is dynamically downloaded locally using `kagglehub`.

### 📥 Download via Python

```python
import kagglehub

# Download latest version of the dataset
path = kagglehub.dataset_download("kundanbedmutha/exam-score-prediction-dataset")

print("Path to dataset files:", path)