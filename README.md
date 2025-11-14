Below is your **GitHub Description** and a complete, professional **README.md** for the project using the Iris dataset + Streamlit + scikit-learn + devcontainer.json.

---

# **GitHub Short Description (≤300 characters)**

Interactive Streamlit app for predicting Iris flower species using a trained RandomForest model. Includes sliders for input features, EDA visualizations, and seamless development through a DevContainer setup for reproducible environments.

---

# **README.md**

# 🌷 Simple Prediction App — Iris Classifier

A Streamlit application that predicts the species of an Iris flower using a trained **RandomForestClassifier**.
The app provides a clean interface for choosing feature values, visualizing dataset statistics, and reviewing model predictions.
This project includes a **DevContainer setup** for reproducible development environments.

---

## Features

* Interactive sliders for **Sepal Length**, **Sepal Width**, **Petal Length**, and **Petal Width**
* Real-time prediction using a trained **RandomForest** model
* Built-in **EDA section** with group statistics and line charts
* Fully containerized development using **devcontainer.json**
* Lightweight, fast, and beginner-friendly

---

## Project Structure

```
/
├── streamlit-iris.py          # Main Streamlit application
├── Iris.csv                   # Dataset
├── devcontainer.json          # VS Code DevContainer setup
├── requirements.txt           # Python dependencies
└── README.md                  # Documentation
```

---

## Getting Started

### 1. Clone Repository

```bash
git clone https://github.com/FouaadAI/streamlit_iris_prediction.git
cd streamlit_iris_prediction
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the App

```bash
streamlit run streamlit-iris.py
```

The app will open automatically in your browser at:

```
http://localhost:8501
```

---

## Using DevContainer (Recommended)

This project includes a ready-to-use **VS Code DevContainer** for isolated and reproducible development.

### Requirements

* VS Code
* DevContainers extension / GitHub Codespaces
* Docker

### Steps

1. Open the project folder in VS Code
2. When prompted: **Reopen in Container**
3. The environment auto-installs:

   * Python 3.11 base image
   * Required libraries from requirements.txt
   * System packages from packages.txt
   * Streamlit launched automatically

The app becomes available on port **8501** and opens through VS Code preview automatically.
Configuration reference:
`devcontainer.json` 

---

## Requirements

Include the following in `requirements.txt`:

```
streamlit
pandas
scikit-learn
```

---

## How It Works

### 1. Load Dataset

The app loads **Iris.csv** and splits data into training/testing sets.

### 2. Build Model

A RandomForest classifier is trained with:

* `max_depth=2`
* `n_estimators=200`
* `max_features=4`

### 3. User Inputs

Sidebar sliders allow users to adjust feature values.

### 4. Predictions

Model predicts the species:

* *Iris-setosa*
* *Iris-versicolor*
* *Iris-virginica*

### 5. EDA

The app computes group means per species and displays:

* Grouped DataFrame
* Line chart of feature means

---

## Output Example

The app shows:

```
Predicted class: Iris-setosa
```

Based on selected slider values.

---

## License

Released under the MIT License.
