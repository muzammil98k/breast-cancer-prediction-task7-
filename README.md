# 🔬 SVM Diagnostic Model for Breast Cancer

An analytical project demonstrating the power of Support Vector Machines (SVM) for building a high-precision binary classification model for medical diagnosis.

---

### **Introduction**
This repository contains a Jupyter Notebook that details the process of creating a predictive model for breast cancer diagnosis. Using the Wisconsin Breast Cancer dataset, we explore the effectiveness of SVMs, tune model parameters for optimal performance, and provide clear visualizations of the results.

### **Analytical Approach**
Our methodology is designed to be rigorous and reproducible:

* **Data Preparation**: We begin by loading the data, encoding the binary 'diagnosis' target, and scaling all numeric features to prevent bias.
* **Kernel Exploration**: We train baseline SVMs with both `linear` and `RBF` kernels to establish an initial performance benchmark.
* **Cross-Validated Tuning**: A `GridSearchCV` is implemented to exhaustively test combinations of `C` and `gamma` parameters, ensuring we find the most robust model configuration.
* **Final Assessment**: The best model is rigorously tested on unseen data, with results presented in a classification report and a confusion matrix.

### **Model Performance**
The final, tuned SVM classifier is highly effective, achieving a test accuracy that underscores its potential for real-world application.

| Metric                  | Result           |
| ----------------------- | ---------------- |
| **Model Type** | SVM (RBF Kernel) |
| **Test Set Accuracy** | **98.6%** |
| **Precision (Malignant)** | 0.98             |
| **Recall (Malignant)** | 0.95             |

> The model excels at correctly identifying malignant cases (high recall), which is critical in a diagnostic setting.

![Grid Search Performance](https://placehold.co/600x400/2c5282/ffffff?text=Hyperparameter+Tuning+Results)

### **Usage Guide**

**Dependencies:**
* Python 3.x
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn

**Instructions:**
1.  Clone the project repository.
    ```sh
    git clone [https://github.com/your-username/svm-diagnostic-model.git](https://github.com/your-username/svm-diagnostic-model.git)
    ```
2.  Navigate into the project directory.
    ```sh
    cd svm-diagnostic-model
    ```
3.  Install necessary libraries.
    ```sh
    pip install pandas scikit-learn matplotlib seaborn
    ```
4.  Launch Jupyter and open the `SVM_Cancer_Analysis.ipynb` notebook to explore the code and results.
