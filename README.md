# ML Projects Repository

Welcome to **ML-Projects**! This repository contains a collection of machine learning and deep learning projects developed using Python. Each project demonstrates a different application of Artificial Intelligence, including predictive modelling, data analysis, anomaly detection, and computer vision.

The objective of this repository is to explore how machine learning algorithms can be used to solve practical problems through data processing, model training, evaluation, and prediction.

## 📂 Projects Included

### 1. Student Grade Prediction System

**Objective:** Predict a student's final examination marks and corresponding grade based on academic performance.

**Technologies Used:**
- Python
- NumPy
- Pandas
- Scikit-learn
- Linear Regression

**Features:**
- Generates a dataset containing 100 student records.
- Uses study hours, attendance, internal marks, and assignment completion as input features.
- Trains a Linear Regression model.
- Evaluates predictions using MSE, MAE, RMSE, and R² score.
- Accepts new student information to predict final marks and grades.

**Model Performance:**

| Evaluation Metric | Result |
|---|---:|
| MSE | 7.324 |
| MAE | 2.530 |
| RMSE | 2.706 |
| R² Score | 0.9274 |

*Note: The dataset is synthetically generated for demonstration purposes.*

---

### 2. Water Quality Monitoring and Prediction System

**Objective:** Analyse water quality parameters and classify water samples according to their potential usability.

**Technologies Used:**
- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Folium

**Machine Learning Algorithms:**
- Random Forest Classifier
- Isolation Forest

**Features:**
- Generates sample water quality data using NumPy.
- Analyses parameters such as:
  - pH
  - Turbidity
  - Dissolved Oxygen (DO)
  - Heavy Metals
  - Temperature
  - Rainfall
- Classifies water into three categories:
  - Safe
  - Irrigation
  - Not Safe
- Detects unusual data patterns using Isolation Forest.
- Visualizes water quality parameters using scatter plots.
- Displays sample locations on an interactive geographical map using Folium.

**Model Performance:**

| Evaluation Metric | Result |
|---|---:|
| Random Forest Accuracy | 90% |

*Note: The current implementation uses synthetic water quality data and simulated geographical coordinates. It is a demonstration model rather than a real-time water monitoring system.*

---

### 3. Dog Vision – Dog Breed Classification

**Objective:** Develop an image classification model capable of identifying dog breeds from uploaded photographs.

**Technologies Used:**
- Python
- TensorFlow
- TensorFlow Hub
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

**Deep Learning Approach:**
- Convolutional Neural Network (CNN)
- Transfer Learning
- MobileNetV2

**Features:**
- Works with the Kaggle Dog Breed Identification dataset.
- Supports classification across 120 different dog breeds.
- Processes and resizes images to 224 × 224 pixels.
- Normalizes image data before model training.
- Creates training, validation, and test batches.
- Uses early stopping and TensorBoard for training monitoring.
- Generates prediction probabilities for each dog breed.
- Exports predictions into a CSV file compatible with the Kaggle competition format.

**Dataset:**

[Kaggle – Dog Breed Identification](https://www.kaggle.com/c/dog-breed-identification/data)

*Note: The current notebook is an experimental implementation. Its validation results are still low, and the model architecture requires further refinement to ensure the output layer consistently supports all 120 breeds.*

---

## 🛠️ Installation and Setup

### Prerequisites

- Python 3.x
- Jupyter Notebook or Google Colab
- Basic understanding of Python and Machine Learning

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/ML-Projects.git
```

### 2. Navigate to the Project Directory

```bash
cd ML-Projects
```

### 3. Install Required Libraries

```bash
pip install numpy pandas scikit-learn matplotlib folium tensorflow tensorflow-hub jupyter
```

### 4. Run the Notebooks

Open Jupyter Notebook:

```bash
jupyter notebook
```

Alternatively, upload the notebooks to Google Colab and execute the cells individually.

**Additional requirement for Dog Vision:**

Download the Dog Breed Identification dataset from Kaggle. The notebook expects the following structure in Google Drive:

```text
DogVision/
├── labels.csv
├── train/
├── test/
├── models/
└── logs/
```

Make sure to configure the dataset paths and Google Drive access before executing the notebook.

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
└── README.md
```

---

## 🎯 Learning Outcomes

Through these projects, the following concepts are explored:

- Data preprocessing and manipulation.
- Exploratory data analysis and visualization.
- Supervised Machine Learning.
- Linear Regression and Random Forest Classification.
- Anomaly detection using Isolation Forest.
- Deep Learning and Neural Networks.
- Transfer Learning using MobileNetV2.
- Model training, testing, and evaluation.
- Image processing and multi-class classification.
- Prediction generation and result visualization.

## 🚀 Future Improvements

- Incorporate real-world datasets instead of relying on synthetic data.
- Improve model performance through hyperparameter tuning.
- Develop a user-friendly interface for prediction and visualization.
- Integrate real-time water quality sensor data.
- Improve the dog breed classification model through better training, validation, and model architecture.
- Deploy trained models as accessible applications or APIs.

## 👨‍💻 Author

**Dibyasis905**

GitHub: [Dibyasis905](https://github.com/Dibyasis905)

---

⭐ If you find these projects interesting, feel free to explore the notebooks and follow the repository for future updates.

**Thank you for visiting ML-Projects!**
