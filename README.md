# uav-location-prediction-xgboost
A repository containing my experiment on implementing XGBoost to create a regression model that can predict the location of a UAV (Latitude, Longitude). It evaluates using [Mean Haversine Distance](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.haversine_distances.html) and achieved 32.9 meters of haversine distance between actual and predicted location. 

### Project description
- **Regression Model**: [XGBRegressor](https://xgboost.readthedocs.io/en/stable/python/python_api.html)
- **Input**: There are total 6440 data with 93 features that are divided into several major categories:
  -  ID, AT (Attitude Information), MAG/COMPASS (Raw Compass, Offset, Compassmot Compensation Values), GPA (Global Position Accuracy), GPS (Global Positioning System), IMU (Inertial Measurement Unit), CTUN (Control, Throttle, and Altitude Information), RCOUT (RC Outputs)
- **Process**: 
    - Exploratory data analysis (EDA).
    - Feature engineering.
    - Modelling.
    - Hyperparameter tuning.
- **Output**: Regression model.

