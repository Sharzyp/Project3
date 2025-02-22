# 📊 Customer Churn Prediction - SyriaTel

## **Overview**
This project aims to predict customer churn for **SyriaTel**, a telecommunications company. By leveraging machine learning models, we identify customers at risk of leaving the service and provide insights to reduce churn rates.

## **1️⃣ Business and Data Understanding**
### **Stakeholder Audience**
- **Business Team**: Needs insights to create customer retention strategies.
- **Data Science Team**: Interested in the model’s accuracy and feature importance.
- **Marketing Team**: Uses churn predictions to optimize targeted offers.

### **Dataset**
The dataset contains customer usage data, billing information, and service plans. Key variables include:
- **International Plan** (Yes/No)
- **Voice Mail Plan** (Yes/No)
- **Total Call Duration** (Day, Evening, Night)
- **Customer Service Calls** (Number of times a customer contacted support)
- **Churn** (Target variable: 1 = Churned, 0 = Not Churned)

## **2️⃣ Modeling**
We tested two machine learning models:
1. **Logistic Regression** (Baseline model)
2. **Decision Tree** (For better feature interpretability)

### **Feature Engineering & Preprocessing**
- Categorical variables were **encoded** using Label Encoding.
- Numerical variables were **standardized** for better model performance.
- The dataset was **split (80/20)** into training and test sets.

## **3️⃣ Evaluation**
### **Performance Metrics**
| Model | Accuracy | AUC Score |
|--------|------------|------------|
| Logistic Regression | 87% | 0.82 |
| Decision Tree | 90% | 0.85 |

### **Confusion Matrix**
- **Decision Tree Confusion Matrix:** 📊 **Higher accuracy, but risk of overfitting**
- **ROC Curve:** 📈 **Decision Tree had a better AUC than Logistic Regression**

### **Feature Importance**
| Feature | Importance Score |
|---------|----------------|
| Customer Service Calls | 0.35 |
| Total Day Minutes | 0.22 |
| Total Evening Calls | 0.18 |

The most influential factor was **customer service calls**, meaning customers who frequently call support are more likely to churn.

## **4️⃣ Conclusion**
### **Findings**
- Customers with **higher customer service calls** have a **higher churn rate**.
- Offering an **international plan** had minimal impact on churn.
- Decision Tree performed **better** than Logistic Regression.

### **Recommendations**
✔ **Target high-risk customers** with proactive engagement.  
✔ **Improve customer support** to reduce churn triggers.  
✔ Consider **loyalty programs** for long-term customer retention.  
 

---

