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
![Gender Distribution](plots/gender_satisfaction.png)

### Age and Satisfaction 🎂😊
- Satisfaction tends to vary across age groups.
![Age and Satisfaction](plots/age_satisfaction.png)

### Inflight Wifi Satisfaction 📶😄
- Passengers rating Inflight wifi service above 3 are more likely to be satisfied.
![Inflight Wifi Satisfaction](plots/wifi_satisfaction.png)

### Seat Comfort Matters! 💺😌
- Passengers giving a seat comfort rating above 3 are generally satisfied.
![Seat Comfort Satisfaction](plots/seat_comfort_satisfaction.png)

### Business Class Satisfaction ✈️👔
- Business class travelers tend to be more satisfied with their flights.
![Business Class Satisfaction](plots/type_travel_satisfaction.png)

### Cleanliness is Key! 🧹😊
- Passengers rating cleanliness above 3 are more likely to be satisfied.
![Cleanliness Satisfaction](plots/cleanliness_satisfaction.png)

### Food and Drink Delight! 🍔🥤😋
- Passengers rating food and drink service above 3 are satisfied.
![Food and Drink Satisfaction](plots/food_drink_satisfaction.png)

## Model Results 📊🤖

| Model                   | Accuracy    | F1 Score      |
| :---------------------- | :----:      | ---:          |
| DecisionTreeClassifier  | 78%         | 0.81          |
| **RandomForestClassifier** | **79%**| **0.81**    |
| LogisticRegression      | 78%         | 0.83          |
| KNeighborsClassifier    | 78%         | 0.84          |
| **XGB**                 | **78%**     | **0.80**      |

 
