# Netflix Customer Churn Prediction

## 📌 Project Overview
This project predicts whether a **Netflix customer will churn (leave the service)** using machine learning with a **Neural Network (Keras Sequential model)**.  
The notebook covers data preprocessing, exploratory data analysis, model training, and evaluation.

---

## 📂 Dataset
- File: `netflix_customer_churn.csv`  
- Key columns used:
  - `gender`  
  - `subscription_type`  
  - `region`  
  - `device`  
  - `monthly_fee`  
  - `payment_method`  
  - `number_of_profiles`  
  - `favorite_genre`  
  - `churned` (Target variable: 1 = churned, 0 = not churned)  

---

## 🔍 Steps in Notebook
1. **Importing Libraries**  
   - Pandas, NumPy, Matplotlib  
   - Scikit-learn (train_test_split, StandardScaler, OneHotEncoder, accuracy_score)  
   - TensorFlow & Keras (Sequential, Dense)  

2. **Data Exploration**  
   - Checked dataset shape, missing values, duplicates  
   - Value counts for categorical features (gender, region, device, payment method, etc.)  

3. **Data Preprocessing**  
   - Dropped `customer_id` column  
   - One-Hot Encoding for categorical columns  
   - Train-test split (80% train, 20% test)  
   - Feature scaling using StandardScaler  

4. **Model Building (Neural Network)**  
   - Sequential model with multiple Dense layers:  
     - Layer 1: 42 neurons, ReLU  
     - Layer 2: 42 neurons, ReLU  
     - Layer 3: 12 neurons, ReLU  
     - Output: 1 neuron, Sigmoid  
   - Optimizer: Adam  
   - Loss: Binary Crossentropy  

5. **Model Training & Evaluation**  
   - Model trained on training dataset  
   - Evaluated using accuracy score on test data  

---

## 📊 Results
- Successfully built and trained a neural network for churn prediction.  
- Model outputs probability of churn (converted to 0 or 1).  
- Accuracy score achieved on test data (check notebook output).  

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   https://github.com/AditiAggarwal21/Netflix-Churn-AI-Model
