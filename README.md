# Breast Cancer Detection Using Image Processing

This project was developed as part of the **ARTI407 – Image Processing** course at **Imam Abdulrahman Bin Faisal University**. It presents a hybrid system combining **classical image processing** and **machine learning** to detect breast cancer in mammogram images.

---

## 📌 Project Summary

We built a pipeline that preprocesses mammogram ROIs, extracts both **shape** and **texture** features, and classifies them using **Random Forest**. The system was tested on the **MIAS Mammography ROIs dataset** and achieved strong accuracy while remaining computationally efficient.

**Key Highlights:**

* **Accuracy:** 83.33% (Testing set)
* **Dataset:** [MIAS Mammography ROIs](https://www.kaggle.com/datasets/annkristinbalve/mias-mammography-rois)
* **Models Used:** Random Forest
* **Tools:** Python, OpenCV, scikit-learn, scikit-image, NumPy, Matplotlib

---

## 🛠 Pipeline

1. **Preprocessing**

   * Grayscale Conversion
   * Gaussian Blurring
   * Histogram Equalization
   * Otsu’s Thresholding
   * Morphological Closing

2. **Feature Extraction**

   * **Shape:** Area, Circularity, Solidity, Extent, Suspicious Region Count, Suspicious Area
   * **Texture:** Contrast, Energy, Homogeneity (via GLCM)

3. **Classification**

   * Random Forest (200 trees, depth-limited to prevent overfitting)

---

## 📊 Results

| Metric    | Value  |
| --------- | ------ |
| Accuracy  | 83.33% |
| Precision | 83%    |
| Recall    | 83%    |
| F1 Score  | 83%    |

Confusion matrices confirmed **low false positives** and **low false negatives**, essential for medical applications.

---

## 📂 Dataset

* **Source:** [Kaggle – MIAS Mammography ROIs](https://www.kaggle.com/datasets/annkristinbalve/mias-mammography-rois)
---

**Main Libraries:**

* OpenCV
* scikit-learn
* scikit-image
* NumPy
* Matplotlib



