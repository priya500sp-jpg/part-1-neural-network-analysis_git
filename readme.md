# Neural Network Fundamentals and Training Behavior Analysis

## Project Overview

This project focuses on building and evaluating a Neural Network model for customer churn prediction using TensorFlow and Keras. The objective is to analyze customer behavior patterns and predict whether a customer is likely to churn.

The project includes:

* Dataset understanding
* Data preprocessing
* Neural network model development
* Model training and evaluation
* Hyperparameter experimentation
* Final reflections on neural network concepts

---

## Dataset Information

Dataset Used:

* `customer_churn_nn.csv`

The dataset contains customer-related information such as:

* Customer region
* Subscription plan type
* Contract type
* Payment method
* Monthly charges
* Login activity
* Support tickets
* Data usage
* Satisfaction score
* Churn status

Target Variable:

* `churn`

  * `0` → Customer retained
  * `1` → Customer churned

---

## Technologies and Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* TensorFlow / Keras
* Jupyter Notebook

---

## Project Workflow

### 1. Dataset Understanding

* Loaded and explored the dataset
* Checked dataset shape and column details
* Identified categorical and numerical features
* Verified missing values
* Generated statistical summaries

### 2. Data Preprocessing

* Encoded categorical variables using Label Encoding
* Split features and target variable
* Performed train-test split
* Applied feature scaling using StandardScaler

### 3. Neural Network Model Building

A Sequential Neural Network model was created using TensorFlow/Keras.

Model Architecture:

* Input Layer
* Hidden Layer 1 → 16 neurons with ReLU activation
* Hidden Layer 2 → 8 neurons with ReLU activation
* Output Layer → 1 neuron with Sigmoid activation

Loss Function:

* Binary Crossentropy

Optimizer:

* Adam

Evaluation Metric:

* Accuracy

---

## Model Training and Evaluation

The model was trained using:

* Epochs: 20
* Batch Size: 32
* Validation Split: 20%

Evaluation techniques:

* Accuracy Score
* Loss Analysis
* Confusion Matrix
* Accuracy and Loss Graphs

---

## Hyperparameter Experimentation

Three different experiments were performed by changing:

* Number of neurons
* Number of epochs
* Batch size

This helped analyze how hyperparameters affect model performance.

---

## Results

The neural network achieved good performance for customer churn prediction.

Key observations:

* Training accuracy improved steadily over epochs
* Validation loss decreased gradually
* Larger neural network architectures slightly improved performance
* Proper preprocessing improved prediction quality

---

## Conclusion

This project demonstrated the implementation of Neural Networks for binary classification problems. Through experimentation and evaluation, the model successfully learned customer behavior patterns and predicted churn effectively.

The project also provided practical understanding of:

* Neural network architecture
* Activation functions
* Hyperparameter tuning
* Model evaluation techniques

---

## Folder Structure

```text
part-1-neural-network-analysis/
│
├── data/
│   └── customer_churn_nn.csv
│
├── results/
│   ├── accuracy_graph.png
│   ├── loss_graph.png
│   └── confusion_matrix.png
│
├── notebook.ipynb
├── README.md
└── requirements.txt
```

---

## How to Run the Project

1. Create virtual environment

```bash
python -m venv venv
```

2. Activate virtual environment

### Windows

```bash
venv\Scripts\activate
```

3. Install dependencies

```bash
pip install -r requirements.txt
```

4. Launch Jupyter Notebook

```bash
jupyter notebook
```

5. Open and run:

* `notebook.ipynb`

---
