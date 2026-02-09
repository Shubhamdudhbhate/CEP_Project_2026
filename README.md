# 🌊 JalDrishti (जलदृष्टी): Village-Level Groundwater Intelligence

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![C++](https://img.shields.io/badge/C++-17%2F20-blue.svg)](https://isocpp.org/)
[![Python](https://img.shields.io/badge/Python-3.10+-green.svg)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/Framework-React-61dafb.svg)](https://reactjs.org/)
[![Status](https://img.shields.io/badge/Build-Passing-brightgreen.svg)]()

### *Predicting Borewell Success and Preventing Financial Loss for Indian Farmers.*

---

## 📖 Table of Contents
1. [Introduction](#-introduction)
2. [The Problem Statement](#-the-problem-statement)
3. [System Architecture](#-system-architecture)
4. [Why C++ & Python?](#-why-c-and-python)
5. [ML Model & Data](#-ml-model--data)
6. [Key Features](#-key-features)
7. [Getting Started](#-getting-started)
8. [Roadmap](#-roadmap)

---

## 📝 Introduction
**JalDrishti** is an end-to-end data intelligence platform that localized national-level water data (India-WRIS) for the common farmer. By analyzing 10 years of historical groundwater fluctuations, our system predicts the feasibility of new borewells, helping farmers avoid the "dry-hole" trap that leads to massive debt.

## ⚠️ The Problem Statement
In India, drilling a borewell costs between ₹50,000 to ₹2,00,000. 
* **The Gap:** Government data is available at the district/state level, but farmers live and work at the **Village level**.
* **The Risk:** Without historical context, 1 in 3 borewells in water-stressed regions fail within a year.
* **The Solution:** A predictive model that uses decadal data to give an "Authority Score" on water availability.

---

## 🏗 System Architecture



### 1. Ingress Layer (Data Collection)
Automated scripts fetch official data from **India-WRIS** (Water Resources Information System) and **CGWB** (Central Ground Water Board).
### 2. Core Processing (C++ Engine)
A high-performance C++ module handles the mathematical crunching of millions of time-series data points to generate village-level averages.
### 3. Intelligence Layer (Python ML)
An LSTM (Long Short-Term Memory) neural network predicts future water table depth based on:
* Historical rainfall patterns.
* Crop cycles in the specific region.
* Past 10-year groundwater trends.
### 4. Presentation Layer (React.js)
A simple, mobile-first dashboard translated into local languages for farmers and local authorities.

---

## ⚙️ Why C++ and Python?
We use a **Hybrid Engine** to ensure both speed and intelligence:

* **C++ for Performance:** - Rapidly sorts and filters 10 years of raw government CSV/XML data.
  - Handles "Computational Geometry" for mapping village coordinates.
  - Near-zero latency for heavy backend calculations.
  
* **Python for Science:** - Leverages `Scikit-learn` and `TensorFlow` for complex groundwater forecasting.
  - Rapid prototyping of data visualization plots (Matplotlib/Seaborn).

---

## 🧠 ML Model & Data
We don't just show current data; we predict the future.
* **Dataset:** 10 Years of official pre-monsoon and post-monsoon water levels.
* **Model Type:** Random Forest Regressor / Time-Series Forecasting.
* **Goal:** To predict the water table depth (in mbgl - meters below ground level) for the next 24 months.

---

## ✨ Key Features
* **📍 Hyper-Local Search:** Enter your Village/Taluka to get an instant report.
* **🔮 Borewell Predictor:** Visual "Meter" showing the probability of finding water.
* **📊 Loss Prevention Calculator:** Estimates the risk of financial loss based on historical depletion rates.
* **🏛️ Authority Portal:** Special login for Gram Panchayat officials to manage collective water usage.

---

## 🚀 Getting Started

### Prerequisites
* **Compiler:** GCC (with C++17 support)
* **Runtime:** Node.js (v18+) & Python (3.10+)
* **Database:** PostgreSQL

### Installation
1. **Clone the project:**
   ```bash
   git clone [https://github.com/shubham-dudhbhate/JalDrishti.git](https://github.com/shubham-dudhbhate/JalDrishti.git)
   cd JalDrishti
