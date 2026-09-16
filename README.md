# ⚡ Power Plant Energy Prediction using ANN

## 📌 Project Overview

This project uses an Artificial Neural Network (ANN) to predict the electrical energy output of a power plant based on environmental and operational conditions.

The model takes four input features — Ambient Temperature (AT), Exhaust Vacuum (V), Ambient Pressure (AP), and Relative Humidity (RH) — and predicts the net electrical energy output (PE).

The ANN model is implemented using PyTorch and trained using the Adam optimizer and Mean Squared Error (MSE) loss function.

---

## 🎯 Objective

The main objective of this project is to build a regression model that can accurately predict power plant energy production based on given environmental conditions.

---

## 📊 Dataset

The dataset contains the following features:

| Feature | Description |
|--------|-------------|
| AT | Ambient Temperature |
| V | Exhaust Vacuum |
| AP | Ambient Pressure |
| RH | Relative Humidity |
| PE | Net Electrical Energy Output |

- `AT`, `V`, `AP`, and `RH` are used as input features.
- `PE` is the target variable.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- PyTorch
- Matplotlib
- Jupyter Notebook

---

## 🔄 Project Workflow

1. Load the power plant dataset.
2. Check for missing values.
3. Separate input features and target variable.
4. Split the dataset into training and testing sets.
5. Standardize input features using `StandardScaler`.
6. Convert the data into PyTorch tensors.
7. Create `TensorDataset` and `DataLoader`.
8. Build an Artificial Neural Network using PyTorch.
9. Train the model using:
   - ReLU activation
   - Adam optimizer
   - Mean Squared Error (MSE) loss
10. Validate the model after each epoch.
11. Save the model with the best validation loss.
12. Evaluate the model using:
   - Training MSE
   - Testing MSE
   - R² Score
13. Compare actual and predicted energy values.

---

## 🧠 ANN Architecture

The Artificial Neural Network consists of:

```text
Input Layer
    ↓
Linear Layer (4 → 6)
    ↓
ReLU
    ↓
Linear Layer (6 → 6)
    ↓
ReLU
    ↓
Output Layer (6 → 1)
    ↓
Predicted Power Output
