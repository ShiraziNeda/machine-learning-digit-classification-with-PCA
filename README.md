# Machine Learning Digit Classification With PCA

This project focuses on classifying handwritten digits using various machine learning algorithms. Principal Component Analysis (PCA) is utilized for dimensionality reduction, enhancing computational efficiency while preserving important features of the dataset.

## Dataset
The dataset used is the **Digits Dataset** from the `sklearn.datasets` module. It contains 1,797 samples of 8x8 grayscale images representing handwritten digits (0-9). Each image is flattened into a feature vector of size 64.

- **Number of samples:** 1,797
- **Feature size:** 64
- **Classes:** 10 (digits 0 to 9)

## Project Workflow

### 1. Data Visualization
The dataset includes images of handwritten digits. 

### 2. Data Preprocessing
- **Train-Test Split:** The dataset is divided into training and testing subsets (70% train, 30% test).
- **Normalization:** The features are scaled to the range [0, 1] using `MinMaxScaler`.

### 3. Dimensionality Reduction with PCA
Principal Component Analysis (PCA) is applied to reduce the feature space from 64 to 32 dimensions while retaining the most significant information.

- **Original dimensions:** 64
- **Reduced dimensions:** 32

### 4. Classification Models
Four machine learning models are trained and evaluated:

1. **Random Forest Classifier**
   - Max Depth: 128
   - Number of Estimators: 256

2. **Support Vector Machine (SVM)**
   - Kernel: Polynomial

3. **Artificial Neural Network (ANN)**
   - Hidden Layer Size: 256
   - Batch Size: 64
   - Learning Rate: Adaptive

4. **K-Nearest Neighbors (KNN)**
   - Number of Neighbors: 8

### 5. Performance Metrics
The models are evaluated using the following metrics:
- **Accuracy**
- **Precision (Weighted)**
- **Recall (Weighted)**

### 6. Results and Comparison
The performance of each model is compared based on training and testing accuracy, precision, and recall. Visual comparisons are made using bar charts for better insights.

## Key Dependencies
- `numpy`
- `matplotlib`
- `sklearn`
- `pandas`

