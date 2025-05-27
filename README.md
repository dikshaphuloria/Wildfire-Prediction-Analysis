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
