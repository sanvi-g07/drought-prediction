# Drought Level Prediction Model

## Project Overview

This project was created to make a machine learning model that could predict the level of drought (which ranges from None to D4, the most extreme type of drought) using meteorological data, such as temperature, humidity, and wind speed. The model was intended to help with earlier drought detection, which could help farmers and communities prepare for and reduce the damage the drought would cause.

## Dataset

Here is a link to the dataset used, as it was too large to upload to GitHub: https://drive.google.com/file/d/1vqiY1dYwiHv82_Ps_3bN6qDk-hGuHc5a/view?usp=sharing 

The dataset used came from Kaggle (https://www.kaggle.com/datasets/cdminix/us-drought-meteorological-data/data), which sourced its data from the U.S. Drought Monitor. The U.S. Drought Monitor provides the level of drought every week along with weather information.

## Problem

Drought is a serious issue severely impacting agriculture and food security. Less rainfall leads to crops not growing well, more pests and diseases for plants, and health problems for livestock, which can increase food costs and harm the economy. Additionally, some areas do not have accurate soil moisture monitoring, affecting drought prediction. Predicting drought from only weather information, which is more widely available, would allow for faster and more accurate prediction so preventative measures could be implemented earlier.    

Sources:

https://www.drought.gov/sectors/agriculture 

https://www.drought.gov/impacts 

https://www.cdc.gov/drought-health/health-implications/index.html 

## Methodology

After exploring and cleaning the data (removing outliers, making columns all numeric, etc.), I determined the most useful factors for predicting the level of drought using Recursive Feature Elimination. Since most drought level data points were in the ‘None’ category rather than D0 to D4, I used the methods SMOTE and Near Miss to balance the data set.

Many types of models were tested, such as Decision Trees, Random Forests, and KNN algorithms, on the data sets. GridSearchCV was utilized to optimize the model.

## Conclusion

The most accurate model overall was the Random Forest without resampling, with an accuracy of 81%. With further modifications and real-time data, this model has the potential to help in earlier detection of droughts, and have a positive impact on agriculture and economy all over the world.


