# 🧠 Panic Attack Data Analysis Dashboard  

### Comprehensive Insights into Panic Attack Severity, Triggers, Symptoms, and Patient Demographics  

### 🔗 Dashboard Link: *(https://app.powerbi.com/view?r=eyJrIjoiNGE5YjhmNzUtYjJlNC00OWVhLWJlOTEtZmUwYTYzOGVmZmNlIiwidCI6IjEzOWQ5NmE0LWUxMzktNDZkMy05MDkwLTU0ZDMxNTBlM2NhMiJ9)*  

---

![Dashboard Preview](https://github.com/user-attachments/assets/8e3473cd-077b-4908-ae3d-8f3f561cbc83) 

![Dashboard Preview](https://github.com/user-attachments/assets/781df22f-2062-4a46-88d4-ce3ccbda25d3)

![Dashboard Preview](https://github.com/user-attachments/assets/7d399af4-85a3-473e-90f7-7c496b08bda4)

![Dashboard Preview](https://github.com/user-attachments/assets/5fe16375-aeea-4ace-a497-72faa3b744e1)

![Dashboard Preview](https://github.com/user-attachments/assets/5d40d87c-c4ca-4eab-9a91-a53453b58dbd)

![Dashboard Preview](https://github.com/user-attachments/assets/1bf87f75-6e62-47da-b13c-a277dff1ca56)

![Dashboard Preview](https://github.com/user-attachments/assets/245ad60a-87c5-49f3-9626-e2c869af33eb)

---

## ❓ Problem Statement  

Panic disorders affect millions of people worldwide, yet identifying **key risk factors, triggers, and symptoms** remains a major challenge for healthcare providers.  
Without structured analysis, it is difficult to:  

- Detect which **demographic groups** (age, gender, medical history) are at highest risk.  
- Understand the **most common triggers** such as caffeine, PTSD, or stress.  
- Track **symptom prevalence** across patients.  
- Monitor **severity and frequency** of panic attacks to guide interventions.  
- Provide actionable insights for **prevention and treatment**.  

---

## 🎯 Business / Healthcare Objective  

The goal of this project is to create an **interactive dashboard** that provides:  

1. **Patient Risk Profiling** – Segmentation of patients based on panic score severity.  
2. **Trigger Analysis** – Identification of top causes leading to panic attacks.  
3. **Symptom Frequency Tracking** – Understanding which symptoms are most common.  
4. **Demographic Insights** – Patterns by age, gender, and medical history.  
5. **Lifestyle Correlations** – Impact of sleep, caffeine, and alcohol consumption on severity.  

✅ These insights help healthcare professionals design **early interventions, lifestyle recommendations, and awareness programs**.  

---

## 🔍 Key Questions Answered  

1. **Severity & Prevalence**  
   - What percentage of patients experience high panic scores?  
   - What is the average duration and frequency of attacks?  

2. **Demographics**  
   - Which **age group** shows the highest panic scores?  
   - How do **gender differences** impact severity?  

3. **Symptoms**  
   - What are the most common symptoms reported (e.g., sweating, dizziness, chest pain)?  
   - How frequently do multiple symptoms overlap?  

4. **Triggers**  
   - Which **factors** (PTSD, caffeine, stress, phobia, social anxiety) are most common?  
   - How many patients have unknown triggers?  

5. **Lifestyle & Medical History**  
   - How do **sleep hours** impact average panic scores?  
   - Does **alcohol/caffeine intake** increase attack frequency?  
   - Which medical histories (depression, anxiety, PTSD) are associated with higher severity?  

---

## ⚙️ Steps Followed  

### **Step 1 – Data Extraction (Snowflake + SQL)** 🗄  
- Connected to the **Snowflake Cloud Data Warehouse** to access patient panic disorder data.  
- Queried relevant tables containing patient demographics, panic scores, symptoms, triggers, and medical history.  
- Filtered data to include **1200 complete patient records** for the year.  
- Exported the cleaned dataset from Snowflake into **Power BI Desktop** for further analysis.  

### **Step 2 – Data Loading in Power BI** 📥  
- Imported dataset into **Power BI Desktop**.  
- Verified data types (numeric for scores, categorical for symptoms/triggers).  
- Established relationships between patient demographics and health records.  

### **Step 3 – Data Quality Check** ✅  
- Removed duplicate patient records.  
- Handled null values for triggers and symptoms.  
- Standardized categories (e.g., sleep hours ranges, caffeine/alcohol levels).  

### **Step 4 – Data Transformation** 🔄  
- Created calculated measures for:  
  - **High / Medium / Low Panic Score categories**.  
  - **Average Frequency of Attacks per Age Group**.  
  - **Symptom distribution** across patients.  
- Aggregated trigger reasons into **major categories**.  

### **Step 5 – Dashboard Design & Visuals** 📊  
- **KPI Cards** – Total Patients, Avg Panic Score, Avg Attack Duration, Avg Frequency.  
- **Donut Chart** – Panic Score Categories (High, Medium, Low).  
- **Bar Chart** – Trigger Reasons (Caffeine, PTSD, Phobia, Stress, Social Anxiety, Unknown).  
- **Bar Chart** – Symptom Prevalence (Sweating, Shortness of Breath, Dizziness, Trembling, Chest Pain).  
- **Scatter Plot / Line** – Sleep Hours vs Avg Panic Score.  
- **Bar Chart** – Medical History vs Panic Score Categories.  
- **Demographics Segmentation** – Age groups, gender distribution, and lifestyle factors.  

---

## 📌 Insights  

**1️⃣ Severity of Panic Attacks**  
- **29.67% of patients** experience **High Panic Scores**.  
- Avg Panic Score = **5.57**; Avg Frequency = **4.41 times**; Avg Duration = **24.39 minutes**.  

**2️⃣ Demographics**  
- **18–30 yrs** show the **highest average panic score (5.71)** and highest attack frequency.  
- Gender distribution indicates both male and female patients are equally impacted.  

**3️⃣ Symptoms**  
- **Sweating (836 patients)** is the most common symptom.  
- Other frequent symptoms: Shortness of Breath (746), Dizziness (620), Trembling (590), Chest Pain (487).  

**4️⃣ Triggers**  
- Top triggers include **Caffeine (202 patients)**, **PTSD (205)**, **Phobia (203)**, **Stress (187)**, and **Social Anxiety (197)**.  
- **206 patients** reported **unknown triggers**, highlighting diagnosis gaps.  

**5️⃣ Lifestyle & Medical History**  
- Patients sleeping **<6 hours** reported **higher panic scores**.  
- **Depression and anxiety patients** had a higher share of severe panic categories.  
- Caffeine intake increased **attack frequency** significantly.  

---

## 💡 Solutions & Healthcare Recommendations  

1. **Target High-Risk Age Group (18–30 yrs)**  
   - Focus interventions and awareness campaigns on young adults.  

2. **Symptom Monitoring**  
   - Educate patients to track early symptoms like sweating and shortness of breath for preventive action.  

3. **Lifestyle Adjustments**  
   - Encourage improved sleep hygiene (>6 hours) and reduced caffeine/alcohol intake.  

4. **Personalized Care**  
   - Patients with **depression/anxiety** history require closer monitoring and tailored treatment.  

5. **Trigger Management**  
   - Raise awareness about lifestyle triggers (caffeine, stress).  
   - Encourage therapy for PTSD and phobia-related cases.  

---

## 🛠 Tools & Technologies Used  

- **Snowflake** – Cloud data warehouse for storing & extracting healthcare data  
- **SQL** – Data extraction & preprocessing in Snowflake  
- **Power BI Desktop** – Dashboard creation, KPIs & visualization  
- **Power Query** – Data transformation & cleaning  
- **DAX** – Calculated measures for panic score categories  
- **Excel & Python** – Validation & exploratory analysis  

---

## 🚀 How to Run  

1. Clone this repository.  
2. Download and open `Panic_Attack_Analysis.pbix` in **Power BI Desktop**.  
3. Use filters (Age, Gender, Trigger, Medical History, Lifestyle factors) for interactive analysis.  

---

## 🙋‍♀️ Author  

**Pragati Kumari**  
_Data Analyst | SQL | Python | Power BI | Excel_  

🔗 [LinkedIn](https://www.linkedin.com/in/pragati-kumari-b60352305)  
🔗 [GitHub](https://github.com/Pragati928)  

---

## 📄 License  

Open for learning and portfolio demonstration. Not for commercial use.  
