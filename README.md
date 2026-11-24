# Machine Learning & Deep Learning Projects

Welcome to **ML-Projects**! 👋

This repository is a collection of hands-on Machine Learning and Deep Learning projects developed using Python. It demonstrates the practical implementation of different AI techniques, from data preprocessing and exploratory data analysis to model development, evaluation, and prediction.

The projects cover real-world problem domains such as healthcare, education, environmental monitoring, computer vision, and predictive price modelling.

The primary objective is to understand how different machine learning algorithms work, how data influences model performance, and how AI techniques can be applied to practical problems.

---

## 📂 Projects Included

### 1. Student Grade Prediction System

**Domain:** Education | **Type:** Supervised Learning – Regression

**Objective:**

Develop a machine learning model that predicts students' examination performance based on academic-related parameters.

**Technologies Used:**
- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

**Algorithm:** Linear Regression

**Key Features:**
- Generates a synthetic dataset of 100 student records.
- Uses academic parameters to estimate student performance.
- Splits the dataset into training and testing sets.
- Trains a Linear Regression model.
- Evaluates predictions using multiple regression metrics.
- Accepts new student inputs and predicts marks and corresponding grades.

**Recorded Model Evaluation:**

| Metric | Result |
|---|---:|
| MSE | 7.3244 |
| MAE | 2.5303 |
| RMSE | 2.7064 |
| R² Score | 0.9274 |

*Note: Results are based on the synthetic dataset generated in the notebook.*

---

### 2. Water Quality Monitoring and Prediction System

**Domain:** Environmental Monitoring | **Type:** Classification and Anomaly Detection

**Objective:**

Build a machine learning system that analyses water quality parameters and categorizes water samples according to their potential usability.

**Technologies Used:**
- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Folium

**Algorithms:**
- Random Forest Classifier
- Isolation Forest
- Label Encoding

**Key Features:**
- Generates synthetic water quality data.
- Analyses parameters such as pH, turbidity, dissolved oxygen, heavy metals, temperature, and rainfall.
- Classifies water samples into three categories:
  - Safe
  - Irrigation
  - Not Safe
- Uses Random Forest for classification.
- Implements Isolation Forest for anomaly detection.
- Visualizes water quality data through graphical representations.
- Uses Folium for interactive geographical visualization.

**Recorded Model Evaluation:**

| Metric | Result |
|---|---:|
| Random Forest Accuracy | 90% |

*Note: The current implementation uses generated data and simulated geographical coordinates. It is a prototype, not a real-time water monitoring solution.*

---

### 3. Dog Vision – Multi-Class Dog Breed Classification

**Domain:** Computer Vision | **Type:** Deep Learning – Image Classification

**Objective:**

Develop an image classification model that identifies dog breeds from photographs.

**Technologies Used:**
- Python
- TensorFlow
- TensorFlow Hub
- Keras
- NumPy
- Pandas
- Matplotlib

**Deep Learning Approach:**
- Convolutional Neural Networks (CNN)
- Transfer Learning
- MobileNetV2

**Dataset:**

[Kaggle – Dog Breed Identification](https://www.kaggle.com/c/dog-breed-identification/data)

**Key Features:**
- Uses the Kaggle Dog Breed Identification dataset.
- Works with a multi-class dog breed classification task involving 120 breeds.
- Converts images into numerical tensors.
- Resizes images to 224 × 224 pixels.
- Normalizes image pixel values.
- Creates training and validation datasets.
- Uses batch processing for efficient image loading.
- Implements TensorBoard for training visualization.
- Uses Early Stopping to control training.
- Saves and reloads trained models.
- Generates prediction probabilities for dog breeds.
- Prepares prediction outputs in Kaggle submission format.

**Current Development Status:**

The notebook contains an experimental MobileNetV2 implementation. Its recorded validation accuracy is very low, and the current five-class output configuration needs to be reconciled with the 120-breed classification task.

Further work is required on the output layer, training configuration, and model evaluation before considering it a reliable breed classifier.

---

### 4. End-to-End Heart Disease Classification

**Domain:** Healthcare | **Type:** Supervised Learning – Binary Classification

**Objective:**

Develop a machine learning model capable of predicting whether a patient is likely to have heart disease based on clinical attributes.

**Dataset:**

The notebook uses the Cleveland Heart Disease dataset from the UCI Machine Learning Repository.

[UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/Heart+Disease)

**Technologies Used:**
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

**Algorithms Explored:**
- Logistic Regression
- K-Nearest Neighbours (KNN)
- Random Forest Classifier

**Key Features:**
- Performs exploratory data analysis (EDA).
- Examines relationships between clinical attributes and heart disease.
- Visualizes correlations and feature distributions.
- Splits data into training and testing sets.
- Compares multiple classification algorithms.
- Performs manual hyperparameter tuning.
- Implements RandomizedSearchCV and GridSearchCV.
- Evaluates models using confusion matrices and classification reports.
- Calculates accuracy, precision, recall, and F1-score.
- Visualizes ROC curves and examines AUC.
- Investigates feature importance.

**Recorded Model Evaluation:**

The tuned Logistic Regression model achieved:

| Metric | Result |
|---|---:|
| Test Accuracy | 88.52% |
| Precision (Class 1) | 0.88 |
| Recall (Class 1) | 0.91 |
| F1-score (Class 1) | 0.89 |

The confusion matrix recorded:

| | Predicted: No Disease | Predicted: Disease |
|---|---:|---:|
| Actual: No Disease | 25 | 4 |
| Actual: Disease | 3 | 29 |

*Note: This is an educational machine learning experiment using a limited dataset. It is not a clinically validated diagnostic system and must not be used for medical decisions.*

---

### 5. Bulldozers Sale Price Prediction

**Domain:** Predictive Analytics | **Type:** Supervised Learning – Regression

**Objective:**

Build a machine learning model that predicts the future sale price of bulldozers based on their characteristics and historical sales information.

**Dataset:**

[Kaggle – Bluebook for Bulldozers](https://www.kaggle.com/c/bluebook-for-bulldozers/data)

**Technologies Used:**
- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

**Algorithm:**
- Random Forest Regressor
- RandomizedSearchCV

**Key Features:**
- Loads training, validation, and testing datasets.
- Performs exploratory data analysis.
- Parses and processes sale dates.
- Extracts date-related features.
- Converts categorical variables into numerical representations.
- Handles missing numerical and categorical values.
- Creates missing-value indicator features.
- Trains a Random Forest Regression model.
- Performs hyperparameter tuning using RandomizedSearchCV.
- Evaluates model performance using MAE, RMSLE, and R².
- Generates sale price predictions for unseen test data.
- Examines feature importance.

**Recorded Model Evaluation:**

The initial Random Forest experiment produced the following validation results:

| Metric | Training | Validation |
|---|---:|---:|
| MAE | 5,561.30 | 7,177.26 |
| RMSLE | 0.2577 | 0.2936 |
| R² Score | 0.8607 | 0.8320 |

*Note: A subsequent hyperparameter search was also performed. Its recorded validation performance was lower than the initial experiment, making further tuning worthwhile.*

---

## 🛠️ Technologies and Tools

The repository explores the following technologies:

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Data Manipulation | NumPy, Pandas |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Deep Learning | TensorFlow, Keras |
| Transfer Learning | MobileNetV2, TensorFlow Hub |
| Anomaly Detection | Isolation Forest |
| Geographical Visualization | Folium |
| Development Environment | Jupyter Notebook, Google Colab |

## ⚙️ Installation and Setup

### Prerequisites

- Python 3.x
- Jupyter Notebook or Google Colab
- Basic understanding of Python and Machine Learning

### 1. Clone the repository

```bash
git clone https://github.com/Dibyasis905/ML-Projects.git
```

### 2. Navigate to the project directory

```bash
cd ML-Projects
```

### 3. Install the required libraries

```bash
pip install numpy pandas matplotlib seaborn scikit-learn folium tensorflow tensorflow-hub jupyter
```

### 4. Run the notebooks

```bash
jupyter notebook
```

Alternatively, open the notebooks directly using Google Colab.

**Dataset requirements:**

- Student Grade Prediction: Dataset is generated within the notebook.
- Water Quality Monitoring: Dataset is generated within the notebook.
- Dog Vision: Requires the Kaggle Dog Breed Identification dataset.
- Heart Disease Classification: Requires the heart disease dataset.
- Bulldozers Sale Price Prediction: Requires the Kaggle Bluebook for Bulldozers dataset.

Some notebooks use Google Drive paths or environment-specific file locations. Update these paths according to your environment before execution.

---

## 📁 Repository Structure

```text
ML-Projects/
│
├── Student_Grade_Prediction_System.ipynb
│
├── Water_Quality_Monitoring_and_Prediction_System.ipynb
│
├── dog_vision.ipynb
│
├── end-to-end-heart-disease-classification.ipynb
│
├── Bulldozers_sale_price.ipynb
│
└── README.md
```

---

## 🎯 Key Learning Outcomes

Through these projects, the repository explores:

- Data preprocessing and exploratory data analysis.
- Supervised and unsupervised learning concepts.
- Regression and classification algorithms.
- Model training, testing, and evaluation.
- Hyperparameter optimization.
- Cross-validation and performance metrics.
- Feature engineering and feature importance.
- Anomaly detection.
- Deep learning and neural networks.
- Transfer learning and image classification.
- Predictive modelling using real-world datasets.
- Data visualization and interpretation of results.

## 🚀 Future Improvements

- Improve model performance through feature engineering and hyperparameter optimization.
- Replace synthetic datasets with real-world data where available.
- Develop interactive interfaces for model predictions.
- Integrate real-time water quality data from sensors.
- Improve the Dog Vision model for all 120 dog breeds.
- Explore advanced ensemble learning techniques.
- Deploy selected models using FastAPI or Flask.
- Develop web-based applications for easier interaction with trained models.

---

## 👨‍💻 Author

**Dibyasis Mishra**

GitHub: [@Dibyasis905](https://github.com/Dibyasis905)

---

⭐ If you find these projects interesting, feel free to explore the notebooks, learn from the implementations, and follow the repository for future updates.

**Thank you for visiting ML-Projects!**
