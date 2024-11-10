# Omdena-Local-challenges

# Machine Learning Model Development for Crop Yield Prediction: Ridge Regression Analysis and Recommendations

In this project, we aimed to develop a machine-learning model capable of predicting crop yields
using both climatic and agricultural data. The primary goal was to predict the yield of crops in
hectares, a critical task for ensuring sustainable agricultural practices and better planning for
food production.


## Documentation

[Documentation](https://linktodocumentation)


## Data Preprocessing 
1. Data Collection 
2. Data clenaing 
3. Feature Engineering 
4. Standardizaton 
5. Train-Test Split
## Model Selection 
In the model selection process, we focused on choosing a regression model that could accurately predict crop yield.
After considering multiple models, we opted for the Ridge Regressor due to its consistent
performance across multiple metrics and its ability to handle multicollinearity.


## Feature selection 
The model was further optimized using forward feature selection,which helped in narrowing down the most important features that contributed significantly to
yield prediction. This step reduced noise and improved the predictive power of the model.
After feature selection, the following features were identified as the most important for the final
model:
- `area_harvested_usda_1000ha`
- `production_usda_1000ha`
- `area_harvested_fao_1000ha`
- `production_fao_1000ha`
- `soil_temp_L1_C`
- `soil_temp_L2_C`
- `soil_temp_L3_C`
- `soil_temp_L4_C`
- `temp_C`
- `precipitation_era5_mm`
- `wind_northward_m_s`
- `soil_water_L2_fraction`
- `soil_water_L4_fraction`
- `precipitation_chirps_mm`
These features were selected based on their impact on predicting the target variable,
`yield_usda_1000ha`. Ridge Regression’s L2 regularization was used to handle multicollinearity among the features.
## Model Evaluation 
Hyperparameter tuning was conducted to improve the accuracy of the Ridge Regressor model,
resulting in enhanced performance metrics as below results:
- `R2 Score`: 0.9487
- `MAE`: 0.0022
- `MSE`: 0.0357
- `RMSE`: 0.0467


## Model App

[Click here for App](https://omdena-maize-agricultural-yield-in-kenya.streamlit.app/)


## Recommendation

- Inclusion of More Data: One of the major limitations of the project was the small dataset used for model training and evaluation. To enhance the model's performance and generalizability, we recommend incorporating more data from diverse sources. Additional historical data on crop yields, climate patterns, and regional conditions will help improve prediction accuracy and reduce potential biases in the model.

- Domain Expertise: While our technical expertise allowed us to build a functional model, we acknowledge that our knowledge of agriculture and crop dynamics was limited. Collaboration with domain experts in agriculture, climatology, and crop science will provide valuable insights that can further refine the feature selection process and model interpretation.

- Testing on More Diverse Locations: The model was primarily trained and tested on specific data ranges. Expanding the testing scope to include different geographic locations with diverse climatic and agricultural conditions will help assess the model's robustness and adaptability.

- Continuous Model Updates: Since crop yield is influenced by ever-changing environmental and market factors, it’s essential to regularly update the model with new data
## Acknowledgements

 - [Omdena](https://www.omdena.com/about)
 - [Maize Production dataset](https://ourworldindata.org/grapher/maize-production?country=USA~CHN~IND~European+Union~RUS~KEN)
 - [High-Accuracy Maize Plot Location and Yield Dataset in East Africa](https://lacunafund.org/datasets/agriculture/)
 - [Climate Data](https://weatherandclimate.com/kenya)

