# 🍽 Smart Canteen Management Decision Support System (SCMDSS)
[Streamlit App](https://canteen-management-decision-system.streamlit.app)
An web application that assists canteen owners in predicting food demand, optimizing menu planning, and reducing food wastage using Machine Learning and data analytics.

---

## 📌 Overview

The Smart Canteen Management Decision Support System (SCMDSS) is designed to support data-driven decision-making in institutional canteens. The system collects structured weekly sales data, learns from historical trends, predicts future demand, and provides actionable recommendations.

Instead of relying on guesswork, canteen owners can use analytical insights to prepare food more accurately and efficiently.

---

## 🎯 Problem Statement

Canteen owners typically estimate food preparation manually. This results in:

* Over-preparation leading to food wastage
* Under-preparation causing shortages
* Poor inventory planning
* Financial inefficiencies

SCMDSS addresses these issues by analyzing past sales along with contextual factors such as weather and exams to predict future demand levels.

---

## 🚀 Features

### 🔐 Role-Based Access Control (RBAC)

* Admin and Owner roles
* Admin approval for new user registrations
* Secure session-based authentication

### 📊 Weekly Sales Data Entry

* Item-wise sales tracking
* Weather and exam condition logging
* Time-slot based demand capture
* Structured weekly data submission

### 🧠 Machine Learning Prediction

* Random Forest Classifier
* Demand classified as:

  * LOW
  * MEDIUM
  * HIGH
* Context-aware forecasting based on:

  * Weather
  * Exam schedule
  * Region
  * Historical sales data

### 📈 Dashboard & Analytics

* Item-wise performance analysis
* Historical trend visualization
* Weekly menu schedule generation
* Demand sensitivity insights

### 💡 Decision Support

* Procurement recommendations
* Item demand ranking
* Context-based reasoning explanations

---

## 🏗 System Architecture

User Interface (Streamlit)
↓
Authentication & Role Control
↓
Data Collection Module
↓
MongoDB Atlas (Cloud Database)
↓
Data Preprocessing Module
↓
Machine Learning Model (Random Forest)
↓
Prediction & Recommendation Engine

---

## 📂 Project Structure

```
CMDSS/
│
├── models/
│   └── rf_classifier.pkl
│
├── pages/
│   ├── home.py
│   ├── Dashboard.py
│   ├── Predictor.py
│   └── data_entry.py
│
├── utils/
│   ├── db_handler.py
│   └── processor.py
│
├── main.py
├── train_model.py
├── requirements.txt
└── README.md
```

---

## 🛠 Technology Stack

* Python – Backend logic and ML implementation
* Streamlit – Web application framework
* MongoDB Atlas – Cloud NoSQL database
* PyMongo – Database connectivity
* Scikit-learn – Machine Learning (Random Forest)
* Pandas – Data preprocessing
* Pickle – Model serialization
* Streamlit Community Cloud – Deployment

---

## 👤 User Roles

### 🛡 Admin

* Approve new users
* Manage user roles
* Monitor system access

### 👨‍🍳 Owner

* Enter weekly sales data
* View analytics dashboard
* Generate demand predictions
* Receive procurement recommendations

---

## 📊 Machine Learning Model

* Algorithm: Random Forest Classifier
* Input Features:

  * Weather
  * Exam Schedule
  * Region
  * Historical Sales Quantity
* Output:

  * LOW
  * MEDIUM
  * HIGH demand classification

The model identifies patterns such as increased demand during exams or higher snack sales during rainy conditions.

---

## ⚙ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone <repository-url>
cd CMDSS
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Configure MongoDB

Create a folder named `.streamlit` and inside it create `secrets.toml`:

```
MONGO_URI = "your_mongodb_connection_string"
DB_NAME = "canteen_db"
```

### 4️⃣ Run the Application

```bash
streamlit run main.py
```

---
## Demo Login Credentials



The following credentials can be used to explore and test the application.



| Role  | User-name                               | Password  |

| ----- | --------------------------------------- | --------- |

| Admin | [admin@test.com](mailto:admin1) | admin123 |

| User  | [user@test.com](mailto:ctrl+coffee)   | ctrl+coffee  |


> **Note:** These accounts are provided solely for demonstration and evaluation purposes. Please do not modify or delete shared test data.
---

## 🔐 Security

* Password hashing (SHA-256)
* Role-based access restriction
* Admin approval workflow
* Secure secret management

---

## 📌 Modules

* Daily Sales Data Collection Module
* Database Integration Module
* Data Preprocessing Module
* Machine Learning Module
* Prediction & Recommendation Module
* Dashboard & Visualization Module
* Deployment Module

---

## 🚀 Future Scope

* Deep learning-based forecasting (LSTM)
* Real-time inventory monitoring
* Email verification and OTP authentication
* Mobile application development
* Multi-branch scalability

---

## 📜 License

Developed for academic and research purposes.




