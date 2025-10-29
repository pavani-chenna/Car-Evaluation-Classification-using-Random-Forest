# 🚗 Car Evaluation Classification using Random Forest  

## 🖼 Project Overview  
This project classifies *car acceptability* based on various categorical features such as buying price, maintenance cost, safety, and capacity.  
Using the *Random Forest Classifier, it predicts whether a car is **Unacceptable, **Acceptable, **Good, or **Very Good*.

---

## 🎯 Objective  
- Perform *Exploratory Data Analysis (EDA)*  
- Encode categorical variables using *Ordinal Encoding*  
- Build and evaluate a *Random Forest Classifier*  
- Identify the *most important features* influencing car acceptability  

---

## 📊 Dataset Information  

*Dataset Source:* UCI Machine Learning Repository  

| Feature | Description |
|----------|-------------|
| buying | Buying price (v-high, high, med, low) |
| maint | Maintenance cost (v-high, high, med, low) |
| door | Number of doors (2, 3, 4, 5-more) |
| persons | Capacity in terms of persons to carry (2, 4, more) |
| lug_boot | Size of luggage boot (small, med, big) |
| safety | Estimated safety of the car (low, med, high) |
| class | Target variable (unacc, acc, good, vgood) |

---

## ⚙ Workflow  

### 1️⃣ Data Loading & Exploration  
- Loaded the dataset using *Pandas*  
- Checked dataset shape, column names, and value distributions  
- Verified no missing values  

### 2️⃣ Feature Engineering  
- Applied *Ordinal Encoding* using category_encoders  
- Split dataset into training and testing sets (67% / 33%)  

### 3️⃣ Model Building  
- Trained *Random Forest Classifier* with:  
  - Default parameters  
  - 100 estimators  

### 4️⃣ Model Evaluation  
- Evaluated using *Accuracy Score, **Confusion Matrix, and **Classification Report*  
- Achieved accuracy of *≈ 98%*

### 5️⃣ Feature Importance  
- Identified key features:  
  - *Safety* (most important)  
  - *Persons*  
  - *Luggage Boot*

---

## 📈 Visualization Example  

```python
sns.barplot(x=feature_scores, y=feature_scores.index)
plt.xlabel("Feature Importance Score")
plt.ylabel("Feature")
plt.title("Visualizing Important Features")
plt.show()

Output Insight:
Safety is the most influential feature in determining car acceptability.


---

🧰 Tech Stack

Tool	Purpose

Python	Programming language
NumPy, Pandas	Data manipulation
Matplotlib, Seaborn	Visualization
Scikit-learn	Model training and evaluation
Category Encoders	Encoding categorical data



---

🧩 Model Performance

Metric	Score

Accuracy	~0.98
Precision	High
Recall	High
Key Feature	Safety



---

📄 Files Included

File	Description

car_evaluation.csv	Dataset file
car_evaluation.ipynb	Main notebook
README.md	Project documentation



---

🚀 Future Enhancements

Perform Hyperparameter Tuning using GridSearchCV

Try XGBoost or Gradient Boosting for comparison

Deploy the model using Streamlit or Flask

Add a dashboard for real-time prediction



---

👩‍💻 Author

Chenna Pavani
Data Science & Machine Learning Enthusiast

🌐 LinkedIn
✉ [Add your email here]


---

⭐ How to Run the Project

# Clone the repository
git clone https://github.com/yourusername/car-evaluation-classification.git  

# Navigate to project directory
cd car-evaluation-classification  

# Install dependencies
pip install -r requirements.txt  

# Run the notebook
jupyter notebook car_evaluation.ipynb


---

🏁 Conclusion

The Random Forest Classifier achieved ~98% accuracy in predicting car acceptability.
Among all features, Safety was identified as the most critical factor influencing the model’s decision.


---

---

Would you like me to also create a short **requirements.txt** file (so it runs easily when cloned)?
