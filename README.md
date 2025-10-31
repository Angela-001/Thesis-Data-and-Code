# Thesis-Data-and-Code
Predictive modeling of precipitation changes in South Carolina
Predicting precipitation is crucial for many sectors, including agricultural planning and climate adaptation. This study investigates precipitation modeling in South Carolina using machine learning techniques and historical data from 2000-2023. Precipitation patterns are influenced by various climatic factors like temperature, seasonality, and atmospheric pressure, but existing models struggle with localized variations due to the state's unique geography. Using NOAA weather and climate datasets, this research compares the performance of regression and classification models in daily precipitation prediction, evaluated using a time-series-based walk-forward cross-validation approach. Regression models generally performed poorly due to the non-linear and seasonal nature of precipitation, with the Random Forest model achieving the best performance (average R² = 0.316). Reframing the task as a classification problem (precipitation versus no precipitation) improved predictive accuracy, with XGBoost achieving the best performance (average F1 score = 0.722). The most influential precipitation predictors identified were Downward Shortwave Radiation, Specific Humidity, Year, Evapotranspiration, and Day. Future work should explore Python time series forecasting libraries such as Darts and ArcGIS Pro’s Forest-based Forecast tool to incorporate deep learning and spatiotemporal features, enabling long-term predictions for future precipitation events. The study highlights key challenges in spatiotemporal precipitation modeling, including class imbalance, temporal, and spatial dependencies. Overall, this work provides a framework for applying machine learning to future precipitation forecasting. It offers a foundation for developing state-specific precipitation forecasting that supports decision-making for climate adaptation, resource management, and disaster preparedness in South Carolina.



## Technologies Used 

- Python 3.10
- Jupyter Notebook
- pandas, numpy, matplotlib, seaborn
- scikit-learn

## Dataset
- Data was sourced via the Southeast Climate Adaptation Science Center (SECASC) Climate Toolbox  (Climate Projections for the Southeast, n.d.)
This tool provides access to gridMET, a dataset of daily high-spatial resolution (~4-km, 1/24th degree) surface meteorological data covering the United States.

- Data Source: Hegewisch, K.C. and Abatzoglou, J.T.. 'Data Download' web tool. Climate Toolbox (https://climatetoolbox.org/), version 2023-02-20. 

- The Dataset includes ~335,000 daily weather records from 44 grid locations across South Carolina, Trained using (2000–2023) data, Tested with 2024 data. 
- Features selected were:
- Precipitation 
- Specific Humidity
- Maximum Relative Humidity
- Downward Shortwave Radiation
- ASCE Alfalfa Reference Evapotranspiration (ETr)
- Wind Speed
- Wind direction


