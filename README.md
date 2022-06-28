# ai-course-project
Project for summer semester 2021/2022 Jagiellonian University AI basics course.

The goal of the project was to create simple flight prices predictor using [kaggle dataset](https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction) based on:
- Airline: The name of the airline company is stored in the airline column.
- Flight: Flight stores information regarding the plane's flight code.
- Source City: City from which the flight takes off.
- Departure Time: This is a derived categorical feature obtained created by grouping time periods into bins. It stores information about the departure time.
- Stops: Stores the number of stops between the source and destination cities.
- Arrival Time: This is a derived categorical feature created by grouping time intervals into bins. Keeps information about the arrival time.
- Destination City: City where the flight will land.
- Class: A categorical feature that contains information on seat class; it has two distinct values: Business and Economy.
- Duration: A continuous feature that displays the overall amount of time it takes to travel between cities in hours.
- Days Left: This is a derived characteristic that is calculated by subtracting the trip date by the booking date.

The models I trained and compared so I could select the best predictor:
- LinearRegression
- Ridge
- Lasso
- ElasticNet
- RandomForestRegressor
- NeuralNet

To find the best params for most of the models I used grid search technique with kfold cross validation.
