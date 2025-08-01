#  Phishing Website Detection Using Machine Learning

A capstone project integrating **machine learning** and **Power BI** to automatically detect phishing websites based on their structural and behavioral attributes. This project demonstrates the power of data science in cybersecurity, emphasizing real-world applications such as threat detection, email filtering, and browser safety.

---


##  Project Overview

This project explores how machine learning can be used to **distinguish phishing websites from legitimate ones** using features extracted from URLs. The solution includes a predictive model as well as an interactive Power BI dashboard for data exploration and communication of results.

---

##  Problem Statement

 **"Can machine learning effectively differentiate between phishing and legitimate websites?"**

Traditional methods such as blacklists or manual reporting are often **reactive and limited**. This project proposes a proactive approach by training a machine learning model to detect phishing attempts based on a variety of URL-based features.

---

##  Dataset

- **Source:** UCI Machine Learning Repository – Phishing Websites Dataset
- https://archive.ics.uci.edu/dataset/327/phishing%20websites
- **Classes:** 
  - Phishing websites (labeled `-1`)
  - Legitimate websites (labeled `1`)
- **Preprocessing Steps:**
  - Converted `.arff` to `.csv`
  - Merged related files 
    ![converted](images/conversion.png)      ![merge](images/merge.png) 
---

##  Tools and Technologies

| Tool         | Purpose                         |
|--------------|----------------------------------|
| Python       | Data cleaning and model training |
| Scikit-learn | Model building and evaluation    |
| Pandas       | Data manipulation                |
| Power BI     | Interactive visualization        |
| CSV          | Final cleaned dataset format     |

---

##  Methodology
 
1. **Data Cleaning:**
   - Removed missing and irrelevant values
   - Encoded categorical features numerically
   ![cleaning](images/cleaning.png) 
2. **Exploratory Data Analysis (EDA):**
   - Identified key trends
   - Checked for class imbalance
    ![EDA](images/eda.png) 
3. **Model Training:**     
   - Applied classification algorithm (e.g., Decision Tree)
   - Evaluated using accuracy, precision, recall
     ![training](images/training.png) 
4. **Power BI Dashboard:**
   - Visualized dataset structure
   - Displayed model insights and prediction results
     ![dashboard](images/distribution.png) 
---

## 📊 Data Visualization

Power BI was used to create an **interactive dashboard** showing:

- Class distribution of phishing vs legitimate URLs
- Feature importance
- Confusion matrix of model performance
- URL patterns with high correlation to phishing
 ![dashboard](images/distribution.png)  ![dashboard](images/perfomance.png)  ![dashboard](images/urlfeatures.png)  ![dashboard](images/interactive.png) 
---


### 🔹 Feature Insights  
*Highlights the most influential features for phishing detection, such as abnormal URLs and SSL state.*

![dashboard](images/urlfeatures.png)

---

### 🔹 Confusion Matrix  
*Displays true positives, false positives, and overall model performance.*

![Confusion Matrix](images/perfomance.png)

---

##  Model Evaluation

The model was evaluated using:

- **Accuracy:** Proportion of correct predictions
- **Confusion Matrix:** Distribution of TP, TN, FP, FN
- **Precision:** How many predicted phishing sites were actually phishing
- **Recall:** How many actual phishing sites were detected
  ![dashboard](images/confusionmatrix.png)

>  The model performed well with **high recall and low false positive rate**, making it suitable for real-world deployment.

---

##  Key Insights

- **Abnormal URL structure** and **SSL certificate absence** were major indicators of phishing.
- Use of **IP addresses** instead of domain names increased phishing likelihood.
- **Legitimate websites** often have more consistent, secure patterns (SSL enabled, no pop-ups, etc.).

---

##  Recommendations

- Integrate model with:
  - **Email spam filters**
  - **Browser plugins**
- Educate users on common phishing traits (e.g., suspicious characters, no SSL)
- Continuously update the dataset with **recent phishing threats**
- Combine with **real-time reputation APIs** for increased accuracy

---

##  Future Work

- Expand dataset to thousands of URLs from global sources
- Apply **Natural Language Processing (NLP)** to webpage text content
- Explore **ensemble models** like Random Forest and XGBoost
- Build a **real-time Power BI dashboard** with live threat monitoring

---

##  Project Files

| File                         | Description                             |
|------------------------------|-----------------------------------------|
| `Bigdata final project.pbix` | Power BI dashboard with all visuals     |
| `phishing_predictions.csv`   | Cleaned dataset used for modeling       |
| `phishing websites.py`       | (Optional) Python code for training     |
| `README.md`                  | This documentation file                 |

---

##  Author

**Name:** GASANA Akariza Leslie  
**ID:** 27413  
**University:** Adventist University of Central Africa 

