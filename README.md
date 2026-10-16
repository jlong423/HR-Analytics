📊 HR Analytics – Employee Attrition Dashboard
A Power BI project analyzing employee attrition using the IBM HR Analytics dataset. 
This dashboard explores key factors that influence employee turnover, helping organizations understand workforce trends and improve retention strategies.

<img width="750" height="540" alt="HR Dashboard" src="https://github.com/user-attachments/assets/4b40fc77-f687-4302-9d04-138cd8fbbfe8" />


🎯 Purpose
This project demonstrates core Power BI skills including data cleaning, data modeling, DAX measures, and interactive dashboard design. 
It is part of my portfolio as I continue developing my skills in data analytics.

📁 Dataset
IBM HR Analytics Employee Attrition Dataset  
Source: Kaggle
Rows: ~1,470
Columns include:

Age

Attrition (Yes/No)

Department

Job Role

Monthly Income

Years at Company

Job Satisfaction

Work-Life Balance

Education

Gender

🛠️ Tools & Techniques
Power BI Desktop

Power Query (data cleaning, transformations)

DAX Measures (KPIs, calculations)

Data Modeling (relationships, calculated columns)

Interactive Visuals & Slicers


📐 Data Preparation
Key cleaning steps:
Converted data types (Age, MonthlyIncome, YearsAtCompany, etc.)

Removed duplicates

Created Age Group column using conditional logic

Ensured Attrition column is properly categorized

Verified relationships and table structure


📏 DAX Measures

Total Employees = COUNTROWS('HR')

Total Attrition = 
CALCULATE(
    COUNTROWS('HR'),
    'HR'[Attrition] = "Yes"
)

Attrition Rate = DIVIDE([Total Attrition], [Total Employees])

Avg Income = AVERAGE('HR'[MonthlyIncome])

Avg Tenure = AVERAGE('HR'[YearsAtCompany])

🔍 Insights
Employees aged 26–35 show the highest attrition.

The Sales department experiences the most turnover.

Lower monthly income correlates with higher attrition.

Employees with lower job satisfaction leave more frequently.

📦 Files Included
HR_Analytics.pbix

🚀 Summary
This project strengthens my Power BI skills and demonstrates my ability to analyze workforce trends using real HR data. It highlights my competency in data cleaning, modeling, DAX, and dashboard storytelling — all essential skills for a data analyst.
