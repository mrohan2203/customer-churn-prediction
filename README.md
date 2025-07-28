
# Customer Churn Prediction with PySpark

This project implements a scalable machine learning pipeline using PySpark to predict customer churn based on behavioral and account data. It is designed for big data environments and demonstrates end-to-end modeling with Apache Spark.

## 🔍 Objective
Predict whether a customer will churn using telco service data by building a distributed pipeline using Spark MLlib.

## 📁 Dataset
- **Telco Customer Churn Dataset**
- Source: [Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn)

## ⚙️ Technologies
- Apache Spark (PySpark)
- Spark MLlib
- Random Forest Classifier
- OneHotEncoder, StringIndexer, VectorAssembler
- CrossValidator, ParamGridBuilder

## 🧪 Features & Workflow
1. **Data Loading**: CSV read using SparkSession.
2. **Data Preprocessing**:
   - Missing value removal
   - Categorical variable encoding
   - Feature scaling and vectorization
3. **Modeling**:
   - Random Forest Classifier
   - Cross-validation with 3 folds
   - AUC-based performance evaluation
4. **Evaluation**:
   - Accuracy and AUC on unseen test set
   - Feature importance for interpretability

## 📈 Results
- Achieved **84% AUC** using Random Forest
- Scaled across thousands of records using Spark's distributed architecture

## 💾 Output
- Trained model can be saved and reused using:
```python
cv_model.write().overwrite().save("churn_model")
```

## 📎 Usage
1. Clone this repo
2. Load dataset into your Spark environment
3. Run `PySpark_Customer_Churn_Project_Template.py`

## 🧠 Learning Highlights
- How to build machine learning pipelines using Spark
- Preprocessing large datasets with Spark’s distributed engine
- Efficient model evaluation and hyperparameter tuning with MLlib

## 📄 License
MIT License

---

For questions or contributions, feel free to connect: [@rohanmuru2203](https://github.com/mrohan2203)
