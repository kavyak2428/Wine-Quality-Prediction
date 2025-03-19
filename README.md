# **Wine Quality Prediction Report**  

## **1. Introduction**  
The goal of this project is to predict the quality of wine based on its **chemical characteristics** using **machine learning models**. The dataset contains features such as **acidity, density, alcohol content**, and others, which influence wine quality.  

## **2. Dataset Description**  
- **Dataset Name**: WineQT.csv  
- **Features**:
  - Fixed acidity
  - Volatile acidity
  - Citric acid
  - Residual sugar
  - Chlorides
  - Free sulfur dioxide
  - Total sulfur dioxide
  - Density
  - pH
  - Sulphates
  - Alcohol  
- **Target Variable**: **Quality** (Ordinal rating from 3 to 8)  

## **3. Key Steps in the Project**  

### **A. Data Preprocessing**  
✅ **Loading the dataset** using Pandas.  
✅ **Handling missing values** (if any).  
✅ **Removing outliers** using IQR method.  
✅ **Scaling features** using MinMaxScaler.  

### **B. Data Visualization**  
✅ **Distribution of wine quality** using `seaborn.countplot()`.  
✅ **Feature correlation analysis** using `seaborn.heatmap()`.  

### **C. Model Training & Evaluation**  
Three classification models were used:  
1. **Random Forest Classifier**  
2. **Stochastic Gradient Descent (SGD) Classifier**  
3. **Support Vector Classifier (SVC)**  

✅ **Splitting data** into 80% training and 20% testing.  
✅ **Training models** on scaled features.  
✅ **Evaluating performance** using **accuracy score & classification report**.  
✅ **Handling class imbalance** using:
   - `class_weight="balanced"` in models.
   - **SMOTE oversampling** (optional).  

### **D. Results & Performance Metrics**  
- **Random Forest Accuracy**: `≈67%` (Best performing model)  
- **SGD Accuracy**: `≈55-60%` (Struggles with class imbalance)  
- **SVC Accuracy**: `≈62-65%` (Performs decently but slower)  

Random Forest outperforms others due to **better handling of complex relationships** in the data.

---

# **Project Requirements**  

## **1. Software Requirements**  
| Software          | Version Recommended  |
|------------------|------------------|
| Python          | 3.10+            |
| NumPy           | 1.26.4            |
| Pandas          | Latest            |
| Scikit-learn    | Latest            |
| Seaborn         | Latest            |
| Matplotlib      | Latest            |
| Imbalanced-learn (for SMOTE) | Latest |

## **2. Hardware Requirements**  
- **RAM**: Minimum 4GB (8GB+ recommended for large datasets)  
- **Processor**: Intel i5/i7 or AMD Ryzen 5/7  
- **Storage**: Minimum **2GB free space**  

## **3. Installation Commands**  
To install the required libraries, run:  
```bash
pip install numpy pandas scikit-learn matplotlib seaborn imbalanced-learn
```

---

# **Conclusion & Next Steps**  
📌 **Conclusion**:  
- **Random Forest** gave the best results.  
- **SGD struggled** due to class imbalance.  
- **SVC was decent** but not the best choice for this dataset.  

🚀 **Next Steps**:
- Try **Hyperparameter Tuning** to improve accuracy.  
- Experiment with **Deep Learning models** (e.g., Neural Networks).  
- Deploy the model using **Flask or Streamlit** for user interaction.  

