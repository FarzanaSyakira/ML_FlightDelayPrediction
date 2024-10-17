# Predicting Flight Delay Using Machine Learning

## 1. Project Overview
This project aims to create a robust predictive model capable of forecasting departure delays exceeding a two-hour threshold, enabling the airline to take preemptive actions and improve on-time departure performance.

## 2. Dataset Description
The dataset contains detailed flight information for a given year, including various features related to flight performance, delays, and cancellations. Below is an overview of the key columns present in the dataset:

- **Target Variable**:
  - `Departure_Delay`: This is the target variable for our prediction model, which represents the delay in minutes for the flight's departure. It was originally named `DepDelayMinutes`. This variable was converted to binary labels to classify whether a flight is significantly delayed.
    "*1" indicates that the flight was delayed by more than 120 minutes, while "0*" indicates that the flight was delayed by 120 minutes or less.

- **Features**:
  - `Year`: The year of the flight.
  - `Month`: The month of the flight.
  - `Flights`: The total number of flights in the dataset for the corresponding year and month.
  - `Cancelled`: Indicates whether the flight was canceled (1 for canceled, 0 for not canceled).
  - `Diverted`: Indicates whether the flight was diverted (1 for diverted, 0 for not diverted).
  - `Day`: The day of the month when the flight occurred.
  - `Origin`: The airport of origin for the flight.
  - `Dest`: The destination airport for the flight.
  - `AirTime`: The total time (in minutes) spent in the air.
  - `Distance`: The distance (in miles) between the origin and destination airports.
  - `WeatherDelay`: Delay (in minutes) attributed to weather conditions.
  - `CarrierDelay`: Delay (in minutes) attributed to the airline carrier.

**Data Modifications**:
- Several columns were deleted or renamed to focus on the most relevant features for training the machine learning model.
- Only a subset of columns was selected based on their importance in predicting flight departure delays.

## 3. Project Structure
**Data**
- 2019 flight dataset.csv              (Raw dataset)
- final_data.csv                       (Preprocessed dataset used for training)

**Notebook**
- FlightDelayPrediction_FarzanaSyakira.ipynb  (Notebook containing all steps)

## 4. Results
The algorithms used in this project are Logistic Regression, XGBoost Classifier, Support Vector Machine and Random Forest. The selected SVM model, trained on historical flight data, has demonstrated superior predictive capabilities in accurately anticipating departure delays exceeding two hours.It stands as a reliable and effective solution for empowering airline operations with actionable insights to mitigate delays and optimize overall operational performance.

## 7. Conclusion and Future Work
The project successfully predicted flight delay.
