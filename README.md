# 📊 **Exploratory Data Analysis on Student Depression**  

This project is part of IBM’s **Exploratory Data Analysis for Machine Learning** course on Coursera. The goal is to analyze a **student depression dataset** obtained from **Kaggle** to uncover patterns related to mental health. Through **data cleaning, visualization, hypothesis testing, and statistical analysis**, this project provides insights into key factors affecting students' well-being.  

---

## **📁 Dataset Overview**  
This dataset, sourced from **[Kaggle](https://www.kaggle.com/datasets/adilshamim8/student-depression-dataset)**, contains several attributes related to student mental health, including:  

- **Academic Pressure** – The level of stress students experience due to studies.  
- **Financial Stress** – Financial difficulties faced by students and their impact.  
- **Sleep Duration** – The number of hours students sleep daily.  
- **Work/Study Hours** – The amount of time spent on work and academic activities.  
- **Depression Levels** – Self-reported symptoms of depression.  
- **Family History of Mental Illness** – Whether a student has a family history of mental disorders.  

By analyzing these factors, we can identify patterns and correlations that can be useful for **mental health interventions** and **policy-making** in educational institutions.  

---

## **🔍 Data Cleaning & Feature Engineering**  
To ensure high data quality, the following steps were taken:  

### **1️⃣ Handling Missing Data**  
- Missing values were **minimal (18 entries)** and replaced using **mean imputation** to avoid data loss.  
- Categorical variables with missing values were **replaced with the mode (most common value)**.  

### **2️⃣ Standardizing Sleep Duration**  
- The dataset originally contained **text-based categories** for sleep duration (e.g., *“Less than 5 hours”*).  
- A function was created to convert these into numerical values:  
  - *Less than 5 hours* → **5**  
  - *5-6 hours* → **5.5**  
  - *7-8 hours* → **7.5**  
  - *More than 8 hours* → **8**  

### **3️⃣ Encoding Categorical Variables**  
- Binary variables such as **“Have you ever had suicidal thoughts?”** and **“Family History of Mental Illness”** were converted into **1 (Yes) and 0 (No)** using **LabelBinarizer** from `sklearn.preprocessing`.  

### **4️⃣ Scaling Numerical Features**  
- Features like **CGPA, Academic Pressure, Sleep Duration, Work/Study Hours, and Financial Stress** were **normalized** using **StandardScaler** to ensure consistency in data distribution.  

---

## **📊 Key Insights & Findings**  
After **Exploratory Data Analysis (EDA)**, several important patterns emerged:  

📌 **Students experiencing high academic pressure tend to have higher depression levels.**  
📌 **Those sleeping less than 5 hours showed increased stress and dissatisfaction.**  
📌 **Financial stress is a major contributing factor to depression among students.**  

These findings suggest that **academic workload management, financial support programs, and promoting healthy sleep habits can improve student well-being.**  

---

## **📈 Hypothesis Formulation & Testing**  
Based on the observed trends, three hypotheses were formulated:  

1️⃣ **Students facing higher academic pressure are more likely to experience depression.**  
2️⃣ **Students with shorter sleep duration are at greater risk of depression.**  
3️⃣ **Financial stress significantly increases depression levels among students.**  

### **🔬 Formal Hypothesis Testing**  
To test **Hypothesis 1**, a **Pearson correlation test** was conducted between **Academic Pressure** and **Depression Levels**:  

✔ **Pearson Correlation Coefficient (r) = 0.475** → Indicates a **moderate positive relationship**.  
✔ **P-value < 0.05** → **Statistically significant**, confirming that higher academic pressure is associated with increased depression levels.  

This analysis highlights the importance of **reducing academic stress** through structured learning schedules and mental health support systems.  

---

## **🚀 Next Steps in Data Analysis**  
To further refine insights and explore more patterns, the next steps include:  

🔹 **Applying Machine Learning Models** to predict students at risk of depression.  
🔹 **Clustering Analysis** to segment students into risk categories based on mental health factors.  
🔹 **Investigating Gender Differences** to analyze whether depression patterns vary by gender.  
🔹 **Time-Series Analysis** (if available) to track how mental health trends evolve over semesters.  

---

## **📌 Data Quality & Additional Data Request**  
### **Assessment of Data Quality**  
📍 The dataset is **clean and well-structured**, but some limitations exist:  
- **Self-reported data** may introduce bias.  
- **Lack of time-based data** prevents analyzing how depression evolves over semesters.  
- **No data on coping mechanisms** limits understanding of student resilience.  

### **Request for Additional Data**  
To enhance analysis, additional data such as:  
✅ **Psychological support access (e.g., counseling sessions attended)**  
✅ **Social support factors (family & peer interactions)**  
✅ **Academic performance history over multiple semesters**  

…would provide **deeper insights into student mental health trends.**  

---

## **📌 How to Run the Project**  
1️⃣ **Clone the repository**  
```bash
git clone https://github.com/yourusername/Student-Depression-EDA.git
cd Student-Depression-EDA
```  
2️⃣ **Install dependencies**  
```bash
pip install -r requirements.txt
```  
3️⃣ **Run the Jupyter Notebook**  
```bash
jupyter notebook
```  

---

## **📬 Contributions & Feedback**  
If you have suggestions or would like to contribute, feel free to:  
✅ Open an **issue**  
✅ Submit a **pull request**  
✅ Reach out via **LinkedIn/GitHub**  

📩 **Let's connect!** [LinkedIn](www.linkedin.com/in/onayifeke-oghenerunor-485235235) | [GitHub](https://github.com/Eddythemachine)  

#DataScience #EDA #MentalHealth #IBM #Coursera #Students #Kaggle 🚀
