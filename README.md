# Drought Level Prediction Model

## Project Overview

This project was created to make a machine learning model that could predict the level of drought (which ranges from None to D4, the most extreme type of drought) using meteorological data, such as temperature, humidity, and wind speed. The model was intended to help with earlier drought detection, which could help farmers and communities prepare for and reduce the damage the drought would cause.

## Dataset

Here is a link to the dataset used, as it was too large to upload to GitHub: https://drive.google.com/file/d/1vqiY1dYwiHv82_Ps_3bN6qDk-hGuHc5a/view?usp=sharing 

The dataset used came from Kaggle (https://www.kaggle.com/datasets/cdminix/us-drought-meteorological-data/data), which sourced its data from the U.S. Drought Monitor. The U.S. Drought Monitor provides the level of drought every week along with weather information.

## Problem

Drought is a serious issue, as it can have severe impacts on agriculture and food security. Less rainfall leads to crops not growing well, more pests and diseases for plants, and health problems for livestock. These issues can lead to the prices of important foods rising, and harm the economy. By more accurately predicting droughts, more preventative measures could be taken to reduce the impact caused by less rainfall, therefore mitigating the economic impact and reducing the risk of food insecurity.   

## Methodology

After exploring and cleaning the data (removing outliers, making columns all numeric, etc.), RFE was used to determine which factors would be the most useful for predicting the level of drought. Additionally, SMOTE and Near Miss were used to balance the data set, as the given data set was imbalanced (most data points were for no drought rather than from D1 to D4), which could affect the accuracy.

Many types of models were tested, such as Decision Trees, Random Forests, and kNN algorithms, on the data sets. GridSearchCV was utilized to tune and optimize the model.

## Conclusion

The most accurate model overall was the Random Forest without resampling, with an accuracy of 81%. With further modifications and real-time data, this model has the potential to help in earlier detection of droughts, and have a positive impact on agriculture and economy all over the world.


