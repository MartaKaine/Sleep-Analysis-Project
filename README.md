# 💤 Sleep, Activity & Cognitive Performance Analysis

## 📌 Overview
This project explores the relationship between sleep, physical activity, and cognitive performance using two real-world datasets.

The goal was to understand how sleep patterns relate to daily activity levels and whether sleep impacts cognitive performance metrics such as reaction time and memory.

---

## 📂 Datasets Used
- **Fitbit Dataset**  
  Daily activity and minute-level sleep data (steps, calories, activity intensity, sleep stages)

- **Sleep Deprivation & Cognitive Performance Dataset**  
  Includes reaction time, memory accuracy, and psychological measures

---

## 🎯 Objectives
- Analyse the relationship between sleep duration and physical activity  
- Investigate sleep quality using sleep efficiency  
- Explore the impact of sleep on cognitive performance  
- Compare behavioural (Fitbit) vs cognitive datasets  

---

## 🛠 Tools & Technologies
- Python (Pandas, NumPy)
- Jupyter Notebook / Google Colab  
- Tableau (data visualisation)  

---

## 🧹 Data Processing & Cleaning

### Fitbit Dataset
- Aggregated **minute-level sleep data** into daily summaries  
- Standardised date formats across multiple tables  
- Merged activity and sleep data using `Id` and `ActivityDate`  
- Removed duplicate records  
- Handled missing values  
- Filtered unrealistic sleep values:
  - Removed records with **sleep < 3 hours**
  - Removed records with **sleep > 12 hours**

### Feature Engineering
- Created **sleep_hours** from minutes asleep  
- Calculated **sleep efficiency**: sleep_efficiency = minutes_asleep / time_in_bed
- Created **sleep categories** (low / normal / high)  
- Extracted **weekday information**  

### Cognitive Dataset
- Validated data consistency and ranges  
- Prepared variables for correlation analysis  
- Standardised column formats  

---

## 📊 Key Insights

### 🧠 Cognitive Performance
- Average sleep duration was **~5.8 hours**, indicating sleep deprivation  
- Sleep showed a **weak relationship with reaction time and accuracy**  
- Suggests cognitive performance is influenced by multiple factors beyond sleep alone  

---

### 🏃 Activity vs Sleep
- **Weak correlation** between physical activity (steps, active minutes) and sleep duration  
- Higher activity levels did **not consistently lead to longer sleep**

---

### 🌙 Sleep Quality (Efficiency)
- Sleep efficiency showed a **stronger relationship with activity levels**  
- More active individuals tended to have **better quality sleep**, rather than longer sleep
- **BMI** and **calorie expenditure** have a weak positive effct on **sleep quality**

---

### ⚖️ Overall Insight
Sleep is important, but its relationship with both physical activity and cognitive performance is **complex and not driven by a single variable**.

---

## 📈 Visualisations
The project includes:
- Correlation heatmaps  
- Scatter plots (e.g. activity vs sleep, efficiency vs activity)  
- Distribution plots (sleep duration)  
- Box plots (sleep patterns by weekday)  

Visualisations were created using **Python and Tableau**.

<img width="1000" height="740" alt="image" src="https://github.com/user-attachments/assets/082d11ca-c537-4095-b745-2f2ee0ed7ac0" />
<img width="1000" height="450" alt="image (1)" src="https://github.com/user-attachments/assets/bc38de7c-e923-436b-8565-8a2aff94c096" />


---

## 🚀 Future Improvements
- Incorporate additional health metrics (e.g. heart rate, BMI)  
- Combine datasets at user level (if compatible)  
- Expand dataset size for stronger statistical analysis  
- Apply statistical testing or machine learning models  

---

## 💡 What I Learned
- Working with messy, real-world time-series data  
- Handling missing values and inconsistent formats  
- Aggregating granular data into meaningful features  
- Performing exploratory data analysis (EDA)  
- Communicating insights through visualisation  

---

## 👩‍💻 Author
Marta – aspiring Data Analyst with a background in Psychology and experience in data-driven operational roles.
