
##FC Barcelona Performance Analysis: Pre & Post Messi Era

📌 Overview

This project analyzes FC Barcelona's performance before and after Lionel Messi's departure by developing two machine learning models using Random Forest Regressor. The models predict the number of goals scored by Barcelona in three seasons with Messi (2018-19, 2019-20, 2020-21) and three seasons without Messi (2021-22, 2022-23, 2023-24).

The analysis focuses on key match statistics such as shots, corners, opponent statistics, fouls, yellow/red cards, and venue effects.

⚙️ Data Processing

Datasets were sourced from La Liga match data from Football Datasets.

Matches where Barcelona played were extracted.

Standardized features so that Barcelona is always the reference team.

Created a binary feature for Venue (Home = 1, Away = 0).

🏗️ Machine Learning Model: Random Forest Regressor

The model is trained separately on pre-Messi and post-Messi data to predict Barcelona's goals per match.

🔹 Features Used:

Shots, Corners, Opponent Shots, Opponent Shots on Target, Fouls, Yellow Cards, Red Cards, Venue

🔹 Target Variable:

Goals scored by Barcelona

🔹 Training Pipeline:

Split Data: 80% training, 20% testing.

Train Random Forest Regressor with 100 trees.

Evaluate using MAE, MSE, RMSE, and R² scores.

Feature Importance Analysis.

📊 Results & Insights

🔹 Pre-Messi Era (2018-2021)

Model Performance:

Mean Absolute Error (MAE): 1.2978

Root Mean Squared Error (RMSE): 1.6000

R² Score: -0.3408 (negative indicates weak predictive power)

Key Features Affecting Goals:

Shots (31.3%)

Opponent Shots (16.8%)

Yellow Cards (13.0%)

Fouls (12.7%)

Observation: Barcelona’s goal-scoring relied more on their attacking statistics (Shots, Corners, and Opponent Shots on Target).

🔹 Post-Messi Era (2021-2024)

Model Performance:

Mean Absolute Error (MAE): 1.4013

Root Mean Squared Error (RMSE): 1.5282

R² Score: -0.8541 (lower predictive accuracy than pre-Messi era)

Key Features Affecting Goals:

Opponent Shots (21.9%)

Shots (21.2%)

Corners (14.8%)

Fouls (14.5%)

Observation: Post-Messi, the team's performance is influenced more by opponent factors (Opponent Shots, Opponent Fouls), indicating Barcelona’s defensive struggles and unpredictability in goal-scoring.

🔥 Key Takeaways:

Messi's presence led to a more attacking playstyle, with shots on target being the most crucial factor.

Post-Messi, Barcelona’s performance is less predictable, with defensive statistics playing a larger role.

Drop in R² score post-Messi suggests greater variability in performance, possibly due to tactical changes.
