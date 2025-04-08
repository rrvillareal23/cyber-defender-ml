# Cyber Intrusion Detection Using Machine Learning

This project applies machine learning models to detect cyber intrusions using the UNSW-NB15 dataset. It includes steps for data preprocessing, feature engineering, model training, evaluation, and tuning to build an effective intrusion detection system (IDS).

## 📁 Project Structure

- **Section 1**: Data Preprocessing & Feature Engineering  
- **Section 2**: Model Training & Validation  
- **Section 3**: Evaluation & Visualization  
- **Conclusion**: Summary of findings and insights

---

## 📦 Frameworks & Libraries Used

### 🧠 Machine Learning
- **`scikit-learn`** – Core ML library for model training, evaluation, and preprocessing  
  Used for:
  - `RandomForestClassifier`, `DecisionTreeClassifier`
  - `GridSearchCV`, `train_test_split`, `Pipeline`
  - Preprocessing with `StandardScaler`, `OneHotEncoder`, `ColumnTransformer`
  - Evaluation with `accuracy_score`, `precision_score`, `recall_score`, `f1_score`, `classification_report`, `confusion_matrix`

### 📊 Data Analysis
- **`pandas`** – Data manipulation and loading datasets
- **`numpy`** – Numerical operations

### 📈 Data Visualization
- **`matplotlib`** – For plotting graphs and heatmaps
- **`seaborn`** – Advanced visualizations like correlation heatmaps and confusion matrices

---

## 🧪 Dataset

The project uses the [UNSW-NB15](https://research.unsw.edu.au/projects/unsw-nb15-dataset) dataset:
- **Training Set**: `UNSW_NB15_training-set.csv`
- **Testing Set**: `UNSW_NB15_testing-set.csv`
- **Feature List**: `UNSW-NB15_features.csv`

---

## 🚀 Project Highlights

### 🔍 Data Preprocessing
- Missing values handled using mean/mode
- Categorical encoding via OneHot and Label Encoding
- Feature scaling with `StandardScaler`

### 🧱 Feature Engineering
- Feature selection based on domain expertise
- One-hot encoding for non-numeric features
- Correlation heatmap used to find impactful features

### 🤖 Model Training
- Primary model: `RandomForestClassifier`
- Baseline model: `DecisionTreeClassifier`
- Stratified train-test split used for balanced class representation

### 🎯 Model Evaluation
- Metrics:
  - Accuracy
  - Precision, Recall, F1-Score (weighted)
  - Confusion Matrix
  - Balanced Accuracy
- Visualization:
  - Correlation heatmap
  - Confusion matrix heatmap
  - ROC curve (optional)

### 🔧 Hyperparameter Tuning
- `GridSearchCV` for tuning decision tree parameters

---

## 📌 Key Learnings

- **Class Imbalance Handling**: Stratified splits and appropriate metrics improved fairness across categories.
- **Model Selection**: Random Forests outperformed simpler decision trees due to their robustness and ensemble nature.
- **Tuning Impact**: Hyperparameter tuning greatly improved model performance and generalization.

---

## 📚 How to Run

1. Clone this repository  
   `git clone https://github.com/yourusername/your-repo.git`

2. Install dependencies  
   ```bash
   pip install -r requirements.txt
