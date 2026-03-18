# Climate-Network-Dashboard


# 🌍 Climate Network: A Multi-Faceted Visual Analytics System

[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org)
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](#)
[![Dataset](https://img.shields.io/badge/dataset-Historical%20Hourly%20Weather%20Data%20\(Kaggle\)-blue)](#)

---

## 📄 Abstract

Understanding complex climate relationships across global weather stations requires more than traditional statistical summaries. This project presents an **interactive visual analytics system** that transforms large-scale weather data into a **climate network representation**.

Cities are represented as nodes, while climate similarity relationships are modeled as edges derived from correlations between temperature patterns. Network analysis techniques such as **betweenness centrality** and **degree centrality** are used to identify influential climate nodes and improve interpretability by reducing visual clutter.

The system is implemented using **Python and Dash**, enabling coordinated multiple views, redundant visual encoding, and interactive filtering. This dashboard supports exploration of relationships between climate variables and network structure, allowing users to discover insights beyond conventional descriptive statistics.

**Keywords:** Climate Network, Visual Analytics, Betweenness Centrality, PCA, Interactive Dashboard.

---

## 📚 Table of Contents

* Motivation
* Dataset
* Features
* Architecture & Tech Stack
* Model & Network Analytics
* Runbook (Reproducibility)
* Usage
* Visualization & Interactions
* Generalization & Validation
* Project Structure
* Future Improvements
* Contributing
* License
* Author

---

## 🎯 Motivation

* Overcome limitations of traditional statistical approaches in analyzing high-dimensional climate datasets
* Provide an interactive platform to discover structural patterns among global weather stations
* Support analytical reasoning through **network-based visual analytics**
* Demonstrate the importance of centrality metrics in environmental data exploration

---

## 📊 Dataset

* **Source:** Historical Hourly Weather Data (Kaggle)
* **Variables Used:** Temperature time-series across multiple cities

### Data Preprocessing

* Handling missing values
* Data normalization
* Feature extraction
* Pairwise correlation computation
* Threshold-based edge generation

> ⚠️ Ensure compliance with Kaggle dataset usage policies.

---

## ⭐ Key Features

✅ Climate network graph visualization
✅ Interactive filtering (time window, region, correlation threshold)
✅ Network centrality analysis
✅ PCA-based dimensionality reduction
✅ Multiple coordinated dashboard views
✅ Time-series exploration for selected cities

---

## 🏗️ Architecture & Tech Stack

**Programming Language:** Python 3.9+
**Framework:** Dash (Plotly)

### Core Libraries

* pandas
* numpy
* scikit-learn
* networkx
* plotly
* dash

### System Workflow

1. Data ingestion and preprocessing
2. Feature extraction using PCA
3. Climate similarity computation
4. Network construction
5. Centrality metric computation
6. Interactive visualization dashboard

---

## 🤖 Model & Network Analytics

### 🌐 Network Construction

* Nodes represent cities
* Edges represent similarity in temperature patterns
* Correlation threshold determines connectivity

### 📌 Centrality Metrics

* **Betweenness Centrality:** Identifies cities acting as bridges in climate relationships
* **Degree Centrality:** Identifies highly connected climate hubs

### 📉 Dimensionality Reduction

* **Principal Component Analysis (PCA)** reduces complexity in temperature time-series data and enhances visualization clarity

---

## ▶️ Runbook (Reproducibility)

### Step 1 — Clone Repository

```bash
git clone (https://github.com/BONANASSER/Climate-Network-Dashboard)
cd climate-network
```

### Step 2 — Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

### Step 3 — Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4 — Run Dashboard

```bash
python app.py
```

Open browser:

```
http://127.0.0.1:8051/
```

---

## 🎨 Visualization & Interactions

* Dynamic network graph layout
* Node highlighting based on centrality scores
* Interactive sliders for correlation threshold
* Dropdown filters for region and time range
* Linked scatter and time-series plots
* Hover tooltips for detailed station metrics

---

## ✅ Notes on Generalization & Validation

* Sensitivity analysis performed on correlation thresholds
* PCA components validated using explained variance ratio
* Network stability tested across different time windows
* Results consistent across multiple subsets of the dataset

---

## 📁 Project Structure

```
climate-network/
│
├── data/
├── notebooks/
├── src/
│   ├── preprocessing.py
│   ├── network_builder.py
│   ├── visualization.py
│
├── app.py
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 🚀 Future Improvements

* Integration with real-time climate data APIs
* Advanced community detection algorithms
* Deployment using Docker / cloud platforms
* Mobile-responsive dashboard interface
* Deep learning-based climate similarity modeling

---

## 🤝 Contributing

Contributions are welcome. Please fork the repository and submit a pull request with clear documentation.

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Bona Nasser**
MSc Data Science
Haramaya University — Ethiopia

---

