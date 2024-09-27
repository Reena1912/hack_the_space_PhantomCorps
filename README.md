# Space Weather Prediction Model

## Project Overview
This project uses a Random Forest Regressor to predict space weather events, focusing on the prediction of the Estimated Kp index (Estimated K). The model takes various solar and geomagnetic features as inputs and forecasts geomagnetic disturbances that could impact critical infrastructure like satellite communications, power grids, and GPS systems.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Target](#target)
- [Model Architecture](#model-architecture)
- [How to Use](#how-to-use)
- [Significance of the Predicted Kp Index](#significance-of-the-predicted-kp-index)
- [Installation](#installation)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Space weather, particularly geomagnetic storms, can disrupt satellite communication, power grids, and GPS systems. To mitigate such risks, this model predicts the Estimated Kp index, which is a measure of global geomagnetic activity.

## Features
These are the input variables that the model uses to make predictions:
- **Radio Flux (10.7 cm)**: Correlates with the sun’s magnetic activity.
- **Sunspot Number**: Represents the count of visible sunspots on the sun’s surface.
- **Sunspot Area**: The total surface area occupied by sunspots.
- **Flares (C, M, X)**: Different types of solar flares, ranging from small to extreme.
- **Middle Latitude A, High Latitude A, Estimated A**: Geomagnetic indices that measure daily geomagnetic activity.

## Target (Predicted Variable)
- **Estimated Kp Index**: A measure of global geomagnetic activity ranging from 0 to 9:
  - **0-1**: Quiet geomagnetic activity.
  - **2-4**: Unsettled to active conditions.
  - **5-9**: Storm levels, with 9 being the most extreme.

## Model Architecture
The model is based on a Random Forest Regressor, a robust machine learning algorithm that aggregates predictions from multiple decision trees to make more accurate predictions. 

By analyzing historical solar and geomagnetic data, the model forecasts the Kp index and provides early warnings for geomagnetic storms.


