# AI & ML Internship Task 9

## Title
Classification with Logistic Regression using Iris Dataset

---

## Objective

The objective of this task is to implement Logistic Regression for multiclass classification using the Iris Dataset.

The task focuses on:

- Exploratory Data Analysis (EDA)
- Data Preprocessing
- Feature Scaling
- Train-Test Split
- Logistic Regression Model Training
- Model Evaluation
- Confusion Matrix Visualization
- Real-Time Prediction

---

## Tools & Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- GitHub

---

## Dataset Used

### Iris Dataset

The Iris dataset is one of the most popular machine learning datasets used for classification tasks.

Dataset File:

```text
Iris.csv
```

### Features

- SepalLengthCm
- SepalWidthCm
- PetalLengthCm
- PetalWidthCm

### Target Variable

```text
Species
```

Classes:

```text
Iris-setosa
Iris-versicolor
Iris-virginica
```

---

## Libraries Used

### Pandas
Used for:
- Loading dataset
- Data preprocessing
- Data analysis

### NumPy
Used for numerical operations.

### Matplotlib
Used for visualizations.

### Seaborn
Used for:
- Pairplots
- Heatmaps
- Confusion Matrix visualization

### Scikit-learn
Used for:
- Label Encoding
- Standard Scaling
- Train-Test Split
- Logistic Regression
- Evaluation Metrics

---

## Tasks Performed

### 1. Loaded Dataset

Loaded the Iris dataset using Pandas.

```python
df = pd.read_csv("Iris.csv")
```

---

### 2. Exploratory Data Analysis (EDA)

Performed dataset exploration using:

```python
df.head()
df.info()
df.shape
df.isnull().sum()
```

Analyzed:
- Dataset structure
- Feature types
- Missing values
- Number of observations

---

### 3. Data Visualization

Generated Pairplots using Seaborn.

```python
sns.pairplot(df, hue="Species")
```

Purpose:

- Understand feature relationships
- Visualize class separation
- Identify patterns

---

### 4. Label Encoding

Converted species names into numerical labels.

Example:

Before:

```text
Iris-setosa
Iris-versicolor
Iris-virginica
```

After:

```text
0
1
2
```

Purpose:

Machine learning algorithms require numerical target values.

---

### 5. Feature Selection

Selected:

```text
SepalLengthCm
SepalWidthCm
PetalLengthCm
PetalWidthCm
```

as input features.

Selected:

```text
Species
```

as target variable.

---

### 6. Feature Scaling

Used:

```python
StandardScaler()
```

Purpose:

- Standardize feature values
- Improve model performance
- Ensure equal feature contribution

---

### 7. Train-Test Split

Used:

```python
train_test_split()
```

Split Ratio:

```text
80% Training
20% Testing
```

Purpose:

- Train model
- Evaluate model on unseen data

---

### 8. Logistic Regression Model

Used:

```python
LogisticRegression()
```

Purpose:

Classify iris flowers into one of three species categories.

---

### 9. Model Prediction

Used:

```python
model.predict()
```

to generate predictions on test data.

---

### 10. Model Evaluation

Evaluated model using:

#### Accuracy Score

Measures overall prediction correctness.

```python
accuracy_score()
```

---

#### F1 Score

Measures balance between Precision and Recall.

```python
f1_score()
```

---

### 11. Confusion Matrix

Generated Confusion Matrix using:

```python
confusion_matrix()
```

Purpose:

- Compare actual vs predicted classes
- Identify classification errors

---

### 12. Confusion Matrix Visualization

Visualized using Seaborn Heatmap.

Purpose:

- Easy interpretation
- Performance analysis

---

### 13. Real-Time Prediction System

Implemented a simple prediction interface where users can enter:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

and receive the predicted Iris species instantly.

Example Output:

```text
Predicted Species:
Iris-setosa
```

---

## Concepts Learned

### Logistic Regression

A supervised machine learning algorithm used for classification tasks.

Although called "Regression", it is mainly used for classification.

---

### Sigmoid Function

Converts model output into probability values between:

```text
0 and 1
```

Used to determine class membership.

---

### Multiclass Classification

Classification involving more than two classes.

Example:

```text
Setosa
Versicolor
Virginica
```

---

### Train-Test Split

Used to evaluate model performance fairly on unseen data.

---

### Feature Scaling

Standardizes feature values and improves model performance.

---

### Accuracy

Measures overall prediction correctness.

Formula:

```text
Correct Predictions / Total Predictions
```

---

### F1 Score

Balances:

- Precision
- Recall

Useful when evaluating classification models.

---

### Confusion Matrix

Displays:

- Correct Predictions
- Incorrect Predictions

for each class.

---

## Key Observations

1. The Iris dataset is well-balanced across classes.

2. Petal features provide stronger separation between flower species.

3. Logistic Regression successfully classified iris flowers with high accuracy.

4. Feature scaling improved model stability.

5. Confusion Matrix showed strong classification performance across all classes.

---

## Outcome

Successfully implemented Logistic Regression on the Iris Dataset.

The project included:

- Data Exploration
- Preprocessing
- Feature Scaling
- Model Training
- Model Evaluation
- Real-Time Prediction

The model effectively classified iris flowers into their correct species.

---

## Files Included

```text
Logistic_Regression_Iris.ipynb
Iris.csv
README.md
```

---

## Repository Name

```text
AI-ML-Internship-Task-9
```

---

## Author

**Arya Chighare**  
Artificial Intelligence & Data Science  
YCCE, Nagpur
