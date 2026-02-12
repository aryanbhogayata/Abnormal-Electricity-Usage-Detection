# ⚡ Intelligent Abnormal Electricity Usage Detection

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)

### 📌 Project Overview
Electricity theft and meter tampering are major challenges for utility companies, leading to significant revenue losses and grid instability. This project leverages **Machine Learning (Random Forest)** to automate the detection of abnormal electricity usage patterns in real-world smart meter data.

By analyzing household characteristics and energy consumption, the model distinguishes between **Normal** and **Abnormal** usage with **~96% accuracy**, providing a scalable solution for revenue protection.

---

## 👥 Team Members
**College:** Dr. Subhash University (DSU)

| Name | Role |
| :--- | :--- |
| **Aryan Bhogayata** | Team Leader |
| **Ananya Goswami** | Member |
| **Ankit Dervaniya** | Member |
| **Sakshi Fadadu** | Member |
| **Kumbhani Vishva** | Member |

---

## 📂 Dataset
The dataset consists of real-world smart meter readings from Kerala, India.
* **Source:** Kaggle (Intelligent Abnormal Electricity Usage Dataset)
* **Size:** ~10,000 records
* **Key Features:**
    * `Actual_Energy(kwh)`: The recorded energy consumption.
    * `House_Area (sqft)`: Size of the dwelling.
    * `Num_Occupants`: Number of people living in the house.
    * `Appliance_Score`: A score representing the number/type of appliances.
    * `Abnormal_Usage`: Target variable (1 = Abnormal, 0 = Normal).

---

## 🛠️ Tech Stack
* **Language:** Python
* **Data Processing:** Pandas, NumPy
* **Visualization:** Seaborn, Matplotlib
* **Machine Learning:** Scikit-Learn (Random Forest Classifier)
* **Environment:** Jupyter Notebook

---

## 📊 Project Workflow
1. **Data Cleaning:** - Removing non-numeric characters (e.g., "kWh") from energy columns.
   - Handling missing values.
2. **Feature Engineering:** - Extracting `Month` and `Day_of_Week` from dates.
   - One-Hot Encoding for categorical variables (`Region_Code`, `Dwelling_Type`).
3. **Model Training:** - Using **Random Forest Classifier** with 100 decision trees.
   - Split: 80% Training, 20% Testing.
4. **Evaluation:** - Assessing performance using Accuracy, Precision, Recall, and Confusion Matrix.

---

## 📈 Results
The model achieved excellent performance on the test set:

* **Accuracy:** **96.3%**
* **Precision (Abnormal Class):** 97%
* **Recall (Abnormal Class):** 93%

### Key Insight
The **Feature Importance** analysis revealed that `Actual_Energy(kwh)` is the strongest predictor of abnormality, followed by `Connected_Load` and `Appliance_Score`. This confirms that the model correctly identifies anomalies based on usage intensity relative to the house profile.

---

## 🚀 How to Run Locally

1. **Clone the Repository**
   ```bash
   git clone [https://github.com/YourUsername/Abnormal-Electricity-Usage-Detection.git](https://github.com/YourUsername/Abnormal-Electricity-Usage-Detection.git)
