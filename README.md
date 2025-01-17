# iHoops-AI-Competition

## Injury Prediction

iHoopInsight, the winning project of the 2024 Orange Hoops Data Science Challenge, focuses on predicting basketball player injuries. Our team designed an advanced machine learning model to compute an injury risk score for each player. By analyzing key performance metrics and muscle imbalances, the model helps identify and mitigate injury risks, empowering coaches and teams to enhance player safety and performance. Our victory was officially featured on the Syracuse University iSchool webpage, highlighting the significance of our achievement.

<img width="577" alt="Screenshot 2025-01-17 at 5 23 18 PM" src="https://github.com/user-attachments/assets/822cfb2c-aa2c-4569-851f-bc88af7f81f7" />

Below is the link 

https://www.linkedin.com/school/ischoolsu/posts/
https://ischool.syracuse.edu/ischool-announces-winners-of-the-orange-hoops-data-science-challenge/

## Introduction

  * Analyze injury risk in basketball players based on key
    performance metrics.
  * Identify and assess risk factors contributing to injuries (e.g.,
    muscle imbalances, performance metrics).
  * Provide actionable insights for injury prevention strategies.
    
## Data Overview

  * Dataset: 2604 records, 14 unique players.
  * Date Range: January 1, 2023 - December 30, 2023.
  * Key Features:
      * Performance metrics (e.g., distance, speed, jump load, heart rate).
      * Muscle imbalances (e.g., hamstring-to-quad ratio, calf imbalance).
      * Injury information (e.g., injury type, body part, recovery time).
  * Missing Data: High percentage of missing values in injury-related columns.

## Exploratory Data Analysis (EDA)

  * Injury Rate: 226 injuries (8.68% injury rate).
  * Hamstring-to-Quad Ratio and Muscle Imbalances are
    significant predictors of injuries.
  * Position Analysis: Guards appear to have higher injury risk
    based on risk scores.
  * Injury Type: Muscle strains and tendonitis are most
    common injuries.

## Injury Risk Model
  
  * Model: Random Forest: Classifier trained to predict injury risks.
  * Metrics:
      * Precision for injured players: 0.32
      * Recall for injured players: 0.98
      * ROC AUC Score: 0.9

## Risk Scores

* Risk Scores assigned based on model predictions.
* Risk Levels: Very Low, Low, Moderate, High
* Example of High-Risk Players:
    * 1. Malik Robinson (Guard): Risk Score 0.76
    * 2. Brandon Mitchell (Guard): Risk Score 0.75
    * 3. Anthony Lopez (Center): Risk Score 0.72
* Risk Level Distribution: Mostly High and Moderate risks.

## Key Takeaways

* Muscle Imbalances (especially Quad and Calf) are the most significant contributors
  to injury risk.
* Forwards & Guards are at higher risk compared to Forwards and Centers.
* Injury prevention strategies should focus on improving muscle balance, particularly
  in the hamstring-to-quad ratio.
* The Injury Risk Model is effective for identifying high-risk players, but further
  calibration and threshold adjustments can improve precision.

## Final Insights

* Based on the results from the analysis, we can conclude the following:
    * **High Risk Players:** Players in the Guard & Forward position tend to have
       the highest Risk Scores. This indicates that Guards might be at a higher
       risk for injuries in the dataset, particularly given their high Hamstring-To-
       Quad Ratio, Quad Imbalance, and Calf Imbalance.
      
    * **Risk Factors:** The Hamstring-To-Quad Ratio, Quad Imbalance, and Calf
      Imbalance are the key contributors to a player's Risk Score. High-risk
      players (with a risk score of 0.7 and above) typically have significantly
      higher values in these metrics.

    * **Overall Distribution:** The distribution of risk levels is relatively skewed
      toward the High and Moderate categories, with only 2 players classified
      as Very Low Risk. This shows that most players in the dataset have some
      degree of injury risk, and muscle imbalances are a significant contributor.
