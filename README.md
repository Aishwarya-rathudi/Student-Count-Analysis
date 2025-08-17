🎓 Student Count Analysis Dashboard

📊 Built with: Tableau Desktop + Microsoft SQL Server

📂 Domain: Education Analytics

🔗 Type: Data Visualization & Insights

✨ Problem Statement

This dashboard helps analyze key factors that impact students’ academic and personal life, such as:

🛌 Sleep Duration

📖 Study Hours

🙂 Study Satisfaction

🎯 Academic Pressure

💰 Financial Stress

By visualizing these metrics, institutions can:

✔ Identify problem areas like low satisfaction, high academic pressure, or lack of sleep

✔ Improve student well-being with data-driven decisions

✔ Monitor overall trends in learning habits & stress management

⚙️ Steps Followed

1️⃣ Data stored in SQL Server and queried for analysis.

2️⃣ Data imported into Tableau Desktop.

3️⃣ Cleaned & prepared data (handled nulls, formatted fields).

4️⃣ Created visuals for each factor:

🔵 Circle chart → Sleep Duration

📈 Line chart → Study Hours

📊 Bar chart → Study Satisfaction

🟪 Square chart → Academic Pressure

<img width="700" height="300" alt="Image" src="https://github.com/user-attachments/assets/8169b70f-b4e8-4c2e-ba16-55a8ee94a6a8" />

🔴 Bubble chart → Financial Stress

5️⃣ Combined all sheets into a single interactive dashboard.

6️⃣ Added formatting, labels, and insights.

🖼️ Dashboard Snapshot

🔍 Insights
🛌 Sleep Duration

5–6 hrs → 123 students

7–8 hrs → 128 students

< 5 hrs → 123 students

8 hrs → 128 students

👉 Students are evenly distributed across sleep patterns.

📖 Study Hours

Range: 0 to 12 hrs

Peak: 10 hrs → 53 students

Average: 6–8 hrs

🙂 Study Satisfaction (Scale 1–5)

Highest: 116 students (Level 4)

Lowest: 86 students (Level 1)

👉 Majority are moderately satisfied.

🎯 Academic Pressure (Scale 1–5)

Max: 125 students (Level 3)

Min: 88 students (Level 2)

👉 Most face moderate pressure.

💰 Financial Stress (Scale 1–5)

Lowest stress (Level 1) → 110 students

Other levels: 94–102 students each

👉 Financial stress is not a major issue.

🗄️ Data Preparation Queries (SQL Server)

-- Sleep Duration distribution

SELECT Sleep_Duration, COUNT(Student_ID) AS Student_Count

FROM Student_Data

GROUP BY Sleep_Duration;

-- Study Hours distribution

SELECT Study_Hours, COUNT(Student_ID) AS Student_Count

FROM Student_Data

GROUP BY Study_Hours

ORDER BY Study_Hours;

-- Study Satisfaction levels

SELECT Study_Satisfaction, COUNT(Student_ID) AS Student_Count

FROM Student_Data

GROUP BY Study_Satisfaction

ORDER BY Study_Satisfaction;

-- Academic Pressure levels

SELECT Academic_Pressure, COUNT(Student_ID) AS Student_Count

FROM Student_Data

GROUP BY Academic_Pressure;

-- Financial Stress levels

SELECT Financial_Stress, COUNT(Student_ID) AS Student_Count

FROM Student_Data

GROUP BY Financial_Stress;

📚 Key Learnings

✅ How to connect SQL Server → Tableau Desktop

✅ Writing SQL queries for aggregation & preparation

✅ Building multi-factor dashboards

✅ Designing storytelling dashboards for insights
