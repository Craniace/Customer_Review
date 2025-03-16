# Passenger Satisfaction Survey 🛫😃😞

## Overview
This repository contains the analysis of an airline passenger satisfaction survey. The goal is to predict whether a passenger is satisfied or dissatisfied based on various features.

These are the following features information about the passengers of an airline:

- `Gender`: male or female
- `Customer type`: regular or non-regular airline customer
- `Age`: the actual age of the passenger
- `Type of travel`: the purpose of the passenger's flight (personal or business travel)
- `Class`: business, economy, economy plus
- `Flight distance`:The flight distance of this journey(km)
- `Inflight wifi service`: satisfaction level with Wi-Fi service on board (0: not rated; 1-5)
- `Departure/Arrival time convenient`: departure/arrival time satisfaction level (0: not rated; 1-5)
- `Ease of Online booking`: online booking satisfaction rate (0: not rated; 1-5)
- `Gate location`: level of satisfaction with the gate location (0: not rated; 1-5)
- `Food and drink`: food and drink satisfaction level (0: not rated; 1-5)
- `Online boarding`: satisfaction level with online boarding (0: not rated; 1-5)
- `Seat comfort`: seat satisfaction level (0: not rated; 1-5)
- `Inflight entertainment`: satisfaction with inflight entertainment (0: not rated; 1-5)
- `On-board service`: level of satisfaction with on-board service (0: not rated; 1-5)
- `Leg room service`: level of satisfaction with leg room service (0: not rated; 1-5)
- `Baggage handling`: level of satisfaction with baggage handling (0: not rated; 1-5)
- `Checkin service`: level of satisfaction with checkin service (0: not rated; 1-5)
- `Inflight service`: level of satisfaction with inflight service (0: not rated; 1-5)
- `Cleanliness`: level of satisfaction with cleanliness (0: not rated; 1-5)
- `Departure delay` in minutes
- `Arrival delay` in minutes

It is necessary to predict which of the two levels of satisfaction with the airline the passenger belongs to:

    Satisfaction
    Neutral or dissatisfied

## Exploratory Data Analysis (EDA) Insights

### Gender Distribution 🚹🚺
- The number of satisfied males and females is nearly equal.
![image](https://github.com/Craniace/Customer_Review/assets/100042684/60ebcc9c-5df3-4cbb-859f-c81074c5f456)

### Age and Satisfaction 🎂😊
- Satisfaction tends to vary across age groups.
![image](https://github.com/Craniace/Customer_Review/assets/100042684/98851ba7-d475-4f7e-a367-6d90a94adbf8)

### Inflight Wifi Satisfaction 📶😄
- Passengers rating Inflight wifi service above 3 are more likely to be satisfied.
![image](https://github.com/Craniace/Customer_Review/assets/100042684/865bd0a9-1d69-47af-b92b-d7fc0d7df6c6)

### Seat Comfort Matters! 💺😌
- Passengers giving a seat comfort rating above 3 are generally satisfied.
![image](https://github.com/Craniace/Customer_Review/assets/100042684/8e683f97-699f-4aa4-9012-8152f0ec6e1e)

### Business Class Satisfaction ✈️👔
- Business class travelers tend to be more satisfied with their flights.
![image](https://github.com/Craniace/Customer_Review/assets/100042684/745d24f0-d2b3-419d-a33d-d2a08606fd6c)

### Cleanliness is Key! 🧹😊
- Passengers rating cleanliness above 3 are more likely to be satisfied.
![image](https://github.com/Craniace/Customer_Review/assets/100042684/0eef8c52-2808-441c-80ef-cd87a2e94ce2)

### Food and Drink Delight! 🍔🥤😋
- Passengers rating food and drink service above 3 are satisfied.
![image](https://github.com/Craniace/Customer_Review/assets/100042684/e79beafb-4ebb-410f-aacd-207bbfec9cbc)


## Model Results 📊🤖

## **Model Comparison**

| Model                  | Precision (Avg) | Recall (Avg) | F1-Score (Avg) | Accuracy | Remarks                                                                 |
|------------------------|----------------|--------------|----------------|----------|------------------------------------------------------------------------|
| **Decision Tree**       | 0.79            | 0.78          | 0.78            | 0.78     | Balanced performance but slight overfitting potential due to similarity in metrics. |
| **Random Forest**       | 0.79            | 0.78          | 0.78            | 0.78     | Consistent with Decision Tree; potential improvement due to ensemble learning.        |
| **Logistic Regression** | 0.78            | 0.78          | 0.78            | 0.78     | Balanced precision and recall; suitable for linearly separable data.                 |
| **KNN**                 | 0.78            | 0.77          | 0.77            | 0.77     | Stronger recall and precision trade-off; performance may degrade with large data.   |
| **XGBoost (XGB)**        | 0.79            | 0.78          | 0.78            | 0.78     | Best potential due to boosting; good trade-off between bias and variance.            |

## **Prediction of Accuracy**
- The models generally converge around **77%–78%** accuracy.  
- **XGBoost** and **Random Forest** are likely to maintain the best performance due to their ensemble nature.  
- **Logistic Regression** is reliable for balanced data, while **KNN** may struggle with scalability.  
- **Final expected accuracy:** Approximately **78%** (with slight improvements possible through hyperparameter tuning).  


 
