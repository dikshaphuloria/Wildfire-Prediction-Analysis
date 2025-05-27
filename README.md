# Wildfire Prediction Analysis

## INTRODUCTION

> Wildfires are growing in both frequency and intensity. This worrying trend is largely linked to global warming, human activities that impact the environment, and natural ecological shifts. The significant damage caused by these events underscores the urgent need for reliable tools that can predict wildfire risk, allowing for better preparation and response. 
>
> This research project aims to improve our ability to forecast wildfire risk, with a specific focus on California, a state that unfortunately experiences severe wildfire seasons. We will utilize historical data combined with environmental information to develop predictive models capable of assessing the likelihood of wildfires. 
>
> Our approach will involve several key steps. Initially, we conducted thorough exploratory data analysis and visualization techniques to gain a deeper understanding of the underlying patterns, relationships, and characteristics within the wildfire dataset. Following this, we performed rigorous feature selection to identify the most relevant and informative predictors for modeling wildfire risk. Subsequently, we built and trained machine learning models designed to forecast wildfire risk in California. Finally, we evaluated and compared the performance of these models using appropriate metrics to identify the most effective and reliable approaches for wildfire risk assessment. The outcomes of this research are expected to contribute valuable insights into the complex dynamics of wildfire occurrence and provide a foundation for developing more accurate and actionable wildfire risk prediction systems. 

 ## Primary Data Source

The various data sources used are listed in the table below:

| **Data**              | **Data Type**         | **Source**                                                                                                                                              | **Time Range** |
|-----------------------|-----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|
| **Fire History**      | CSV                   | Fire and Resource Assessment Program (FRAP), CAL Fire, United States Forest Service, MSDA Project, Bureau of Land Management, and National Park Service | 2009–2023      |
| **Weather Details**   | Open-Meteo API        | Retrieved historical weather data for specific latitude and longitude coordinates using an open-source weather API                                      | 2009–2023      |
| **Terrain Information** | Google Earth Engine (GEE) | Google Earth Engine was used to obtain topographic and surface information, aiding wildfire prediction by incorporating terrain and vegetation data       | 2009–2023      |
| **Drought Index**     | Google Earth Engine (GEE) | Google Earth Engine was used to collect precipitation and drought index data                                                                             | 2009–2023      |
| **Vegetation/Fuel Type** | Google Earth Engine (GEE) | Google Earth Engine was used to extract vegetation and fuel type information                                                                             | 2009–2023      |

## Results

> This project successfully demonstrates the predictability of wildfire duration using environmental factors such as temperature, topography, and fuel availability. The models built all have an R2 value of greater than 0.70, which shows that we can reliably predict how long a fire is likely to burn. However, predicting the wildfire spread is comparatively more complex due to the dynamic nature of fire spread- heavily influenced by volatile factors like wind speed and terrain slope. Despite the inherent noise in the data, we could achieve a Misclassification Rate of 0.38 using a Random Forest Model using a classification approach. Although the XGB model gives a reasonable accuracy on train data (Error Rate ~0.33), the test error rate is high (~0.5), which shows that the model is overfitting. It is to be noted that the XGB model was only tuned with a limited number of hyperparameters, which showed no significant improvements, and rigorous hyperparameter tuning should be carried out to utilize the predictive power of gradient boosted models.

## Our Project Summary Can be Found:
> 
> Visualization: https://dikshaphuloria.github.io/Wildfire-Prediction-Analysis/Code/DataVisualization.nb.html
> METHODOLOGY (Fire Duration Prediction): https://dikshaphuloria.github.io/Wildfire-Prediction-Analysis/Code/fire_duration_filtered_data.html
> METHODOLOGY (Number of Acres Burnt Prediction): https://dikshaphuloria.github.io/Wildfire-Prediction-Analysis/Code/num_acres_burnt.html
