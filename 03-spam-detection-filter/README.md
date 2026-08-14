## Summary

### Pipeline & Methodology
* **Data Cleaning & EDA:** Explored the dataset and removed duplicate entries.
* **Text Preprocessing & Feature Extraction:** Utilized `CountVectorizer` (Bag-of-Words) to convert raw text into numerical feature vectors.
* **Model Training:** Trained a **Multinomial Naive Bayes** classifier on the vectorized text data.

### Results 
* **Accuracy:** Achieved **~98% accuracy** on the test set.
* **Performance:** The model performed exceptionally well on *Ham* messages, with a slightly lower recall when detecting certain complex *Spam* patterns.
* **Conclusion:** Demonstrates that Multinomial Naive Bayes remains a fast, lightweight, and highly effective baseline for SMS spam detection.