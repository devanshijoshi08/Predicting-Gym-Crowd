## Gym Equipment Utilization Project

### Overview
The Gym Equipment Utilization project is an analytical and predictive modeling endeavor aimed at understanding and forecasting gym crowdedness. Using historical gym attendance data, we build various machine learning models to predict the number of people in the gym at any given time, providing insights that can help manage gym space and equipment effectively.

### Data
The project utilizes the "Gym Crowd" dataset, which comprises records of gym attendance over time, along with other contextual information such as date, time, temperature, and academic calendar indicators.

### Features
- `number_people`: Count of people present in the gym
- `timestamp`: Time of the record
- `day_of_week`: Day of the week as an integer (0 = Monday, 6 = Sunday)
- `is_weekend`: Indicator for whether the day is a weekend
- `is_holiday`: Indicator for holidays
- `temperature`: Ambient temperature
- `is_start_of_semester`: Indicates the start of an academic semester
- `is_during_semester`: Indicates if the date falls during an academic semester
- `month`: Month of the year
- `hour`: Hour of the day when the record was taken

### Installation
To set up the project environment, run the following command to install the required Python packages:
```bash
pip install -r requirements.txt
```

### Data Exploration
Key insights drawn from the initial data exploration include:
- Gym attendance peaks during the evening on weekdays.
- Warmer temperatures and academic semesters tend to correlate with increased gym usage.
- Gym attendance is consistent throughout the year with slight increases at the beginning and near the end of the year.

### Model Training and Evaluation
Several models were trained and evaluated, including:
- Linear Regression
- Decision Tree
- XGBoost
- Random Forest

### Selected Model
The Optimized Random Forest model was selected for its accuracy, generalization capability, and insightful feature importance ranking. 

### Insights from Model
- The timestamp of visits was found to be the most significant predictor, indicating specific times associated with higher attendance.
- The hour of the day was important, reflecting patterns such as pre/post-work gym usage.
- Temperature and academic calendar features also played a role in predicting gym crowdedness.

### Strategies for Gym Management
Based on the model's insights, the following strategies are proposed:
- Implement a reservation system to manage peak-hour equipment availability.
- Offer post-work fitness classes or sessions during peak evening hours.
- Introduce weather-responsive scheduling for classes and staffing.
- Promote indoor gym activities during adverse weather conditions to attract members.

### Viewing the analysis 
Open the `gymCrowdPrediction.ipynb` in jupyter notebook to view the analysis 