# World Cup 2026 Player Performance Analysis (Data Analyst Project)

A beginner-friendly data analysis project for **B.Tech / BCA 1st Year – Data Analyst** learners.
It analyses what drives goal contributions (goals + assists) of players in a World Cup tournament using Python, pandas, matplotlib and seaborn.

> The dataset is **synthetic** (computer-generated). It contains no real player names or real statistics.

## Business problem
A national team's coaching staff and scouting analysts want to know which factors go with goals plus assists in a tournament, so they can decide who to start, how to use substitutes, and which players to scout next.

## Questions answered
1. What does `Goal_Contributions` look like overall?
2. Do `Minutes_Played` and `Shots_On_Target` affect `Goal_Contributions`?
3. Does `Goal_Contributions` differ by `Position`, `Confederation`, `Preferred_Foot` and `Squad_Role`?
4. Which players need attention? A "Quiet Tournament" player has `Goal_Contributions` = 0, and players with 400 or more minutes get special attention.

## Dataset
`wc2026_data.csv` – 255 rows, 12 columns (Player_ID, Position, Confederation, Preferred_Foot, Squad_Role, Age, Minutes_Played, Shots_On_Target, Pass_Accuracy_Pct, Market_Value_Million_EUR, Last_Match_Date, Goal_Contributions).
The raw file intentionally has missing values, duplicates, inconsistent text and impossible values so you can practise cleaning.

## Project structure
```
world-cup-2026-player-performance/
├── data/
│   ├── raw/wc2026_data.csv
│   └── processed/wc2026_clean.csv
├── notebooks/day1 day3.ipynb/day2 day4.ipynb
├── images/                  (charts saved by the notebook)
└── README.md
```

## How to run
```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook notebooks/.ipynb
```

## Steps followed
1. Load and inspect data  2. Clean data (duplicates, text, impossible values, missing values)  3. Create new columns (Contributions_Per_90, Impact_Band, Passing_Band)  4. Exploratory analysis with charts  5. Insights and recommendations

## Key findings (from this dataset)
- Average goal contributions per player ≈ 1.6 (median 1.5).
- Minutes played (correlation ≈ 0.4) and shots on target (≈ 0.5) both show a positive relationship with goal contributions.
- Forwards contribute the most on average (≈ 2.3) and defenders the least (≈ 1.3).
- Starters average ≈ 2.1 contributions compared with ≈ 0.8 for substitutes.
- About 25% of players (63 of 250) had a Quiet Tournament, and 12 of them played 400 or more minutes.

## Charts
![Overall](images/01_overall_performance.png)
![Goal contributions](images/02_goal_contributions_distribution.png)
![Quiet players](images/03_quiet_players_by_position.png)

## Tools
Python 3 · pandas · NumPy · matplotlib · seaborn · Jupyter Notebook

## Author
Samrat Sagar – B.Tech 1st Year (Roll No: 2026B01010931)

