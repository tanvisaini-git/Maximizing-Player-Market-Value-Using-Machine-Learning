# Maximizing Player Market Value and Club Valuation Using Machine Learning
Developed as a part of the Modern Analytics class at Duke University's Business Analytics Program. It was a team project created by Liuxinhao Gao, Akshay Navada, Tanvi Saini, Mike Shu, and Nina Wu.

## Overview
This project leverages machine learning to help selling football clubs like Ajax and Brighton optimize player development and maximize transfer profits. By analyzing data from Kaggle on over 2,000 players, we developed predictive models using Linear Regression, Lasso, and Random Forest to estimate player market value.

The model provides insights into trainable attributes that increase market value for attackers, midfielders, and defenders, enabling clubs to: <br>
  ✔️ Tailor training programs to enhance high-value skills. <br>
  ✔️ Strategically time player sales to maximize transfer fees.<br>
  ✔️ Make data-driven valuation decisions for better return on investment (ROI).

## Motivation
The football transfer market is worth over €6.5 billion, with selling clubs playing a pivotal role in developing and transferring top talent. These clubs rely heavily on player sales, but identifying the right attributes to focus on during training remains a challenge. Our project provides a data-driven solution to:

* Pinpoint which player attributes contribute most to market value.
* Identify overvalued players to sell at peak price.
* Accurately assess rising talents to negotiate better transfer deals.

## Data Sources & Feature Engineering
📊 Dataset: Football Players’ Transfer Fee Prediction Dataset
🔗 Dataset Link

### Key Features:
* Performance Metrics (Goals, Assists, Passes, etc.)
* Market Value & Transfer Fees
* Player Position (Attack, Midfield, Defense)
* League-Specific Impact
* Weighted Aggregation of Seasonal Stats
### Feature Engineering:<br>
✔ Handling Missing Values (Logical imputation & weighted season-based averaging).<br>
✔ Position-Based Segmentation (Clustering to separate attackers, midfielders, and defenders).<br>
✔ Data Cleaning (Syntax corrections, encoding categorical variables, and outlier removal).

## Modeling Approach
We tested three machine learning models to predict player market value:

* Linear Regression – Simple and interpretable but sensitive to multicollinearity.
* Lasso Regression – Best performer; improves feature selection and reduces complexity.
* Random Forest – Strong predictive power but less interpretable.<br>
📌 Best Model: Lasso Regression (lowest RMSE across all player categories).

## Key Insights & Strategic Coaching Recommendations
### Attackers (Forwards & Strikers)
🔹 Top Attributes:

* Expected Goals per 90 min (xG/90)
* Non-Penalty Goals
* Penalty Kicks Won<br>
✅ Coaching Focus: Enhance finishing drills, one-on-one attacking, and positioning in the penalty box.
### Midfielders
🔹 Top Attributes:

* Expected Assists per 90 min (xA/90)
* Passes Leading to Goals
* Total Assists<br>
✅ Coaching Focus: Prioritize vision, passing accuracy, and goal-creating actions. Loaning players to top leagues significantly boosts market value.
### Defenders
🔹 Top Attributes:

* Number of Times Received Pass
* Total Carries
* Touches in Midfield Third<br>
✅ Coaching Focus: Develop ball-playing defenders, improve tactical positioning, and enhance passing under pressure.

## Deployment & Future Enhancements
### Current Impact:
* Train players based on high-value attributes.
* Market value predictions help clubs time transfers for maximum profit.
* Data-driven valuation insights refine negotiation strategies.
### Future Scope:
🔹 Expand Player Metrics – Incorporate physical attributes (e.g., height, weight, and goalkeeping stats).<br>
🔹 Optimize Transfer Timing – Build a price volatility model to predict best-selling periods.<br>
🔹 Balanced Training Approach – Ensure holistic player development without over-prioritizing market-driven attributes.<br>

By leveraging machine learning, selling clubs can outperform competitors, refine scouting strategies, and maximize ROI on player transfers.
