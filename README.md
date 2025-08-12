# 🏏 IPL Performance Insights Dashboard (2021–2023)

🔗 **Live Dashboard:** [View on Power BI](https://app.powerbi.com/groups/me/reports/f814c0dc-d595-4dda-961c-7bf700a8d5bf/0b85073aea70e3a5d2a3?experience=power-bi)

---

## 📖 Project Background
This project was created as part of a **Resume Challenge** simulating a real-world sports analytics requirement.

**Scenario:**  
"Sports Basics", a sports blog company, wanted to boost their website traffic with a **special edition IPL 2024 magazine**.  
The magazine’s goal: provide **interesting insights and facts** for **fans, analysts, and teams**, based on the **last 3 years (2021–2023)** of IPL data.

The **Chief Editor**, Tony Sharma, tasked **Peter Pandey** (a fictional, data-savvy cricket journalist) with designing an **interactive dashboard** that answers key questions, reveals trends, and delivers visually appealing stats for the magazine.

**My Role:**  
I stepped into the shoes of Peter Pandey to analyze IPL data, extract meaningful insights, and create a **Power BI dashboard** that could be used directly in the magazine’s analytics section.

---

## 🚀 Key Objectives
- Summarize team & player performance from **2021 to 2023**
- Highlight **top batsmen, bowlers, and all-rounders**
- Compare **chasing vs defending win rates**
- Identify **best bowlers** and **best batsmen** based on defined criteria
- Provide **seasonal trends** and **match-wise breakdowns**
- Include **predictions for IPL 2024**
- Make the dashboard **interactive and easy to explore**

---

## 📊 Features
- **Season-wise** and **overall** performance comparison  
- **Custom KPIs**: Boundary %, Strike Rate, Economy Rate, Dot Ball %  
- **Dynamic slicers** for year, team, and player  
- **Top performers** leaderboards for batting, bowling, and all-round performance  
- **Win Analysis**: Chasing vs Defending  
- **2024 Predictions**: Top 4 teams, Orange Cap, Purple Cap  
- **Best XI** team selection  
- **Interactive tooltips** for deeper insights  
- **Match-level drilldowns** for detailed performance  

---

## 📂 Dataset & Sources
Dataset provided as part of the Resume Challenge:  
- `dim_match_summary`  
- `dimPlayers`  
- `fact_batting_summary`  
- `fact_bowling_summary`  

Additional research-based inputs were included for KPI calculations.  
**Note:** Data covers **2021–2023 IPL seasons** only.

---

## 🛠 Data Transformation & Measures
Performed in **Power Query** & **DAX**:
- Cleaned null values and duplicates  
- Applied filters:
  - Batting → minimum 60 balls faced
  - Bowling → minimum 60 balls bowled
- Established relationships between tables for accurate aggregations  
- Created **DAX measures** for key KPIs:
  ```DAX
  Boundary% = DIVIDE([Total Fours] + [Total Sixes], [Balls Faced])
  DotBall% = DIVIDE([Dot Balls], [Balls Bowled])
  Bowling SR = DIVIDE([Balls Bowled], [Wickets Taken])
  Win Rate (Chasing) = DIVIDE([Wins Chasing], [Matches Chasing])
  Win Rate (Defending) = DIVIDE([Wins Defending], [Matches Defending])

🖼 Dashboard Pages
The dashboard contains 7 interactive pages, each focusing on a specific analysis area:

Home Page 🏠

Central navigation hub linking to all other pages.

Quick overview of dashboard sections.

Team Analysis 🏏

Season-wise and overall performance of each team (2021–2023).

Win/loss trends, chasing vs defending stats, and consistency metrics.

Batting Analysis 🏆

Performance review of batsmen across all three seasons.

KPIs: Boundary %, Batting Strike Rate, Total Runs, and 50+/100+ scores.

Bowling Analysis 🎯

Performance review of bowlers across all three seasons.

KPIs: Economy Rate, Bowling Strike Rate, Dot Ball %, and Wickets Taken.

2024 Predictions 🔮

Predicted Top 4 teams, Orange Cap holder, and Purple Cap holder based on past 3 seasons’ performance.

Best XI ⭐

Probable combined playing XI for the last 3 seasons:

4 Batters

1 Wicketkeeper

2 All-rounders

2 Spinners

2 Fast Bowlers

Top 3 All-rounders 💪

Detailed comparison of the best 3 all-rounders from the last 3 seasons based on combined batting and bowling metrics.

📌 How to Use
Open the 📐 Ranking Criteria
Best All-rounder → Min. 100 balls faced & 60 balls bowled, highest combined batting & bowling score.
Best Spinner → Economy + Wickets + Dot Ball % (spin type only).
Best Pacer → Strike Rate + Wickets + Dot Ball % (pace type only).

🖼 Dashboard Pages
The dashboard contains 7 interactive pages, each focusing on a specific analysis area:

Home Page 🏠

Central navigation hub linking to all other pages.

Quick overview of dashboard sections.

Team Analysis 🏏

Season-wise and overall performance of each team (2021–2023).

Win/loss trends, chasing vs defending stats, and consistency metrics.

Batting Analysis 🏆

Performance review of batsmen across all three seasons.

KPIs: Boundary %, Batting Strike Rate, Total Runs, and 50+/100+ scores.

Bowling Analysis 🎯

Performance review of bowlers across all three seasons.

KPIs: Economy Rate, Bowling Strike Rate, Dot Ball %, and Wickets Taken.

2024 Predictions 🔮

Predicted Top 4 teams, Orange Cap holder, and Purple Cap holder based on past 3 seasons’ performance.

Best XI ⭐

Probable combined playing XI for the last 3 seasons:

4 Batters

1 Wicketkeeper

2 All-rounders

2 Spinners

2 Fast Bowlers

Top 3 All-rounders 💪

Detailed comparison of the best 3 all-rounders from the last 3 seasons based on combined batting and bowling metrics.

📌 How to Use
Open the Live Dashboard.

Select Season from slicer (2021, 2022, 2023, or All).

Use Team, Stage and Player filters for focused insights.

Hover over Player names for interactive tooltips.

👤 Author
Jayram Prabhu
📧 Email: prabhujayram1010@gmail.com
🔗 LinkedIn: https://www.linkedin.com/in/jayram-prabhu-5326a6182/
💻 GitHub: 

