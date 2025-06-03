
# 🐧 K-Nearest Neighbors (KNN) Classification – Penguins Dataset

## 📌 Objective
Apply and understand the K-Nearest Neighbors (KNN) algorithm using the **Palmer Penguins dataset** to classify penguin species.

---

## 🧰 Tools Used
- **Seaborn** (for loading dataset)
- **Pandas**
- **Scikit-learn**
- **Matplotlib**

---

## 📊 Dataset Description

The Penguins dataset is a modern replacement for the Iris dataset and provides information on three penguin species: **Adelie, Gentoo, and Chinstrap**.

### Features used:
- `bill_length_mm`
- `bill_depth_mm`
- `flipper_length_mm`
- `body_mass_g`

The target is the `species` column.

---

## 🧭 Steps Followed

### 1. **Load and Clean the Dataset**
- Load dataset via `seaborn.load_dataset("penguins")`
- Drop rows with missing values using `dropna()`

### 2. **Preprocess the Data**
- Encode categorical labels (`species`) using `pd.factorize()`
- Normalize the numerical features using `StandardScaler`

### 3. **Split the Data**
- Divide data into training and testing sets (70% / 30%) using `train_test_split()`

### 4. **Train KNN Classifier**
- Train `KNeighborsClassifier` with values of **K from 1 to 10**
- Evaluate each model using accuracy

### 5. **Visualize Accuracy vs K**
- Plot accuracy across different values of K to choose the best one

### 6. **Evaluate Best Model**
- Select best-performing K based on accuracy
- Generate and display a **confusion matrix** to evaluate classification performance

---

## ✅ Observations

- Best K selected using accuracy metric
- Model performs well with proper scaling and cleaned dataset

---

## 📎 Notes

- This dataset is slightly more realistic than Iris and includes some missing values and mixed types
- Ideal for practicing classification with real-world biological data

---

## 🔗 Reference
- [Palmer Penguins Dataset](https://allisonhorst.github.io/palmerpenguins/)
