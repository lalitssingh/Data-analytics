# 📊 Data Analytics Portfolio

Welcome to my **Data Analytics Portfolio**!  
This repository highlights my end-to-end data analysis projects, covering data cleaning, transformation, visualization, and storytelling.  

I’ve showcased **three projects** that demonstrate my skills in Python, SQL, Tableau, and Figma.

---

## 🚀 Featured Projects

---

### 1️⃣ HR Analytics Dashboard  
**Tools Used:** Tableau · SQL · Figma  

#### 🔹 Objective  
To design a comprehensive HR Dashboard that provides insights into hiring trends, workforce demographics, and income patterns, enabling HR managers to make data-driven decisions.  

#### 🔹 Data Collection & Cleaning (SQL)  
- Cleaned raw HR dataset using SQL queries.  
- Removed duplicates, handled missing values, and standardized job titles.  

```sql
-- Removing duplicate employee records
DELETE FROM employees
WHERE rowid NOT IN (
    SELECT MIN(rowid)
    FROM employees
    GROUP BY employee_id
);

-- Handling missing department values
UPDATE employees
SET department = 'Unknown'
WHERE department IS NULL;

🔹 Visualization & Design
Built in Tableau, structured into:
Overview: hires, terminations, active employees
Workforce Breakdown: department, job title, HQ vs. branches
Demographics: gender ratio, age groups, education levels
Income Analysis: salary by gender, education, and department
Designed a clean dashboard background in Figma for better visual storytelling.

🔹 Key Insights
Gender-based salary disparities exist in higher education groups.
Branch offices had more employees compared to HQ.
Education strongly correlated with performance ratings.
