# CEP_Project_2026

# 🌊 JalDrishti (जलदृष्टी)
### *Advanced Village-Level Groundwater Analytics & Predictive Modeling*

![Project Header Animation](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNHJpZ3Z4bmZ6eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4JmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZ力を/3o7TKMGpxx8G3S5X6U/giphy.gif) 
*(Note: Replace with a custom GIF of your dashboard in action later)*

---

## 📖 Project Vision
**JalDrishti** is a mission-driven platform designed to solve the "Dry Borewell" crisis in rural India. By synthesizing 10 years of official data from **India-WRIS** and **CGWB**, we provide farmers with high-precision groundwater predictions. 

Instead of guessing where to drill, farmers get a **probability-based success score**, saving them lakhs of rupees in failed infrastructure costs.



---

## 🛠️ Detailed System Architecture

### 1. Data Ingestion Layer (The "Ingress")
* **Source:** India-WRIS (Water Resources Information System).
* **Scale:** 10 Years of historical time-series data.
* **Format:** Automated scrapers converting PDF/Table data into structured **PostgreSQL** entries.

### 2. The Prediction Engine (ML Logic)
We utilize a **Time-Series Analysis** approach to predict future water levels.
* **Algorithms:** LSTM (Long Short-Term Memory) or Random Forest Regressor.
* **Features:** Historical rainfall, soil type, previous year's water table, and village-level extraction rates.
* **Output:** Predicted water level in meters below ground level (mbgl).

### 3. High-Performance Processing (C++ Core)
For heavy mathematical computations and data sorting across millions of rows of historical village data, we use a C++ backend module to ensure near-instant results.

---

## 🚀 Key Modules & Visuals

### 📍 Village-Level Mapping
| Feature | Description |
| :--- | :--- |
| **Borewell Predictor** | Enter coordinates to see the success probability. |
| **Historical Trends** | Animated graphs showing water depletion over the last decade. |
| **Authority Dashboard** | Real-time map for Gov officials to track village health. |

---

## 💻 Tech Stack & Tools

![Tech Animation](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExZnd3Znd3Znd3Znd3Znd3Znd3Znd3Znd3Znd3Znd3Znd3JmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZ力を/S60Cr90mNis8YVmgY8/giphy.gif)

* **Frontend:** React.js + Tailwind CSS (for a mobile-first farmer UI).
* **Backend:** Node.js (API) + C++ (Processing).
* **Data Science:** Python (Pandas, Scikit-learn, Matplotlib).
* **Database:** Supabase / PostgreSQL.
* **DevOps:** Git/GitHub for version control.

---

## 📈 ML Pipeline Animation
1. **Raw Data** (India-WRIS) ➔ 2. **Cleaning** (Null removal) ➔ 3. **Training** (10-Year History) ➔ 4. **Inference** (Farmer Query)

---

## 🛠️ Development Setup

### Prerequisites
* **C++ Compiler** (GCC/Clang)
* **Python 3.10+**
* **Node.js v18+**

### Local Installation
```bash
# 1. Clone the repository
git clone [https://github.com/shubham-dudhbhate/JalDrishti.git](https://github.com/shubham-dudhbhate/JalDrishti.git)

# 2. Setup ML Environment
cd ml-engine
pip install -r requirements.txt

# 3. Start the UI
cd ../client
npm install && npm start
