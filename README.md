# ⚓ Sonar Rock vs Mine Prediction

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Overview
This machine learning project aims to detect whether a sonar signal indicates a **Mine (M)** or a **Rock (R)**. Using a binary classification approach with **Logistic Regression**, the model analyzes 60 distinct frequencies to identify potential underwater threats.

## 📂 Dataset Details
* **Source File:** `sonar dataset.csv`
* **Dimensions:** 208 rows, 61 columns.
* **Features (X):** 60 numerical attributes representing the energy of sonar returns at different angles.
* **Target (Y):** Column 60, containing labels 'R' (Rock) or 'M' (Mine).

## 🛠️ Technologies & Libraries
The project is built using Python and the following data science stack:
* **Pandas:** For loading and manipulating the dataset (`read_csv`, `describe`).
* **NumPy:** For array manipulation and reshaping input data for prediction.
* **Scikit-Learn:**
    * `train_test_split`: To split data into training and testing sets.
    * `LogisticRegression`: The core classification algorithm.
    * `accuracy_score`: To evaluate model performance.

## ⚙️ Project Workflow
1.  **Data Loading:** Importing the dataset without a header (`header=None`).
2.  **Preprocessing:**
    * Separating features (X) and target (Y).
    * Splitting data with `test_size=0.1` (10% for testing) and `stratify=Y` to maintain class balance.
3.  **Model Training:** Fitting the Logistic Regression model on the training data.
4.  **Evaluation:** Calculating accuracy scores to check for overfitting.
5.  **Prediction System:** A custom block to predict new instances by reshaping input arrays (`(1, -1)`).

## 📊 Results & Performance
The model achieved the following accuracy scores:
* **Training Accuracy:** **83.42%**
* **Test Accuracy:** **76.19%**

*> Note: The difference suggests a need for a larger dataset to improve generalization, as indicated in the notebook comments.*

## 💻 How to Run
1.  Clone the repository:
    ```bash
    git clone [https://github.com/KAMILELH/sonar-rock-vs-mine.git](https://github.com/KAMILELH/sonar-rock-vs-mine.git)
    ```
2.  Install dependencies:
    ```bash
    pip install pandas numpy scikit-learn
    ```
3.  Run the Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

## 👤 Author
**Kamil El Harbili**
* Student @ FSTM
* [GitHub Profile](https://github.com/KAMILELH)
