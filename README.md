# Deloitte Forage Virtual Internship

## Overview
The **Deloitte Forage Virtual Internship** provided hands-on experience with real-world business problems, allowing me to apply data analysis and visualization techniques to solve key challenges faced by companies. This internship focused on working with structured and unstructured data to derive meaningful insights for decision-making.

Throughout the internship, I completed multiple tasks that involved data analysis, visualization, and classification using tools like **Tableau** and **Excel**. Below is a detailed breakdown of the tasks I completed.

---

## Task 1: Telemetry Data Analysis in Tableau

### **Background**
Daikibo, an industrial manufacturing company, collected telemetry data from four factories worldwide:
- **Factory Meiyo** (Tokyo, Japan)
- **Factory Seiko** (Osaka, Japan)
- **Daikibo Berlin** (Berlin, Germany)
- **Daikibo Shenzhen** (Shenzhen, China)

Each factory had **9 types of machines**, generating telemetry messages every **10 minutes** over a one-month period (**May 2021**). The goal was to analyze machine failures to answer two key questions:
1. Which factory had the most machine breakdowns?
2. Which machines broke down most frequently in that location?

### **Approach**
1. **Imported the JSON telemetry data** into **Tableau**.
2. **Created a calculated field** called `Unhealthy`, assigning a value of **10** to unhealthy machine statuses (representing 10 minutes of potential downtime per message).
3. **Built visualizations**:
   - **Bar chart:** "Down Time per Factory" to compare machine downtime across factories.
   - **Bar chart:** "Down Time per Device Type" to show breakdowns by machine type.
4. **Designed an interactive dashboard**:
   - Linked both charts to allow filtering by factory.
   - Enabled dynamic insights by selecting a factory to view its machine downtime details.
5. **Identified the factory with the highest downtime** and captured a screenshot for submission.

### **Tableau Dashboard**  
Here is the interactive Tableau dashboard I created for Task 1:
![Alt Text](https://github.com/tanish314/Deloitte-Forage-Virtual-Internship/blob/main/Task%20One/Dashboard.png)

## Task 2: Gender Pay Equality Classification in Excel

### **Background**
Daikibo received **internal complaints about gender pay inequality** across different job roles and locations. The **Forensic Tech Team** developed an algorithm to compute an **Equality Score** for each job role, where:
- **0** indicates perfect equality.
- **Negative values** indicate gender pay disparity against women.
- **Positive values** indicate gender pay disparity against men.
- Scores range from **-100 to +100**.

### **Approach**
1. **Imported the "Equality Table.xlsx" dataset**, which contained:
   - `Factory`
   - `Job Role`
   - `Equality Score`
2. **Created a new column, "Equality Class", to categorize the scores using an Excel formula**:
   ```excel
   =IF(ABS(C2) <= 10, "Fair", IF(ABS(C2) <= 20, "Unfair", "Highly Discriminative"))
   ```
3. **Classification Logic**:
   - **Fair:** Scores between **-10 and +10**
   - **Unfair:** Scores between **-20 and -11** OR **11 and 20**
   - **Highly Discriminative:** Scores below **-20** or above **+20**
4. **Saved and submitted the updated file** with the classification applied to all job roles.

---

## Key Learnings
Through this virtual internship, I gained valuable experience in:
- **Data visualization**: Creating insightful dashboards using Tableau to drive data-driven decisions.
- **Data classification and automation**: Using Excel formulas to efficiently categorize data.
- **Analytical problem-solving**: Identifying patterns and key insights from complex datasets.
- **Interpreting business problems**: Translating raw data into meaningful recommendations for stakeholders.

---

## Conclusion
The **Deloitte Forage Virtual Internship** provided an opportunity to work on practical data analytics problems faced by businesses. Through tasks involving **Tableau** and **Excel**, I enhanced my ability to analyze, visualize, and interpret data effectively. These skills are crucial for roles in **data science, business intelligence, and analytics**.
