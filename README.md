#### Project Objective

The objective of this project was to determine if environmental factors influence estimates of white-tailed deer density.  The results of this study were intended to improve TMD’s data accuracy and logistics of annual spotlight deer surveys. 

#### Methods: 

Spotlight survey data was collected by the Department of the Interior in Great Smoky Mountains National Park from 1993-2003.  The spotlight survey route was within Cades Cove, Townsend, TN 378882.

#### Results: 

The environmental factors below do not significantly influence estimates of deer density made from spotlight surveys. Temperature was found to be the most influential predictor from a simple linear regression model (SLR) and two optimized machine learning models (i.e., random forest and gradient boosting optimized via GridSearchCV). The R<sup>2</sup> (i.e., proportion of variance explained by the model) of the selected linear model was poor (~ 0.10).  However, temperature was found to be a statistically significant predictor (p < 0.001).  The selected SLR found that for every 1 degree fahreheit increase in temperature, there was a 0.80 decrease in the deer density. Environmental factors: 

* month of the year (numerical)
* temperature (numerical)
* wind (boolean)
* cloud cover (categorical)
* rain (boolean)
* snow (boolean)
* fog (boolean)
* moon phase (categorical)

#### Management Implications: 

Environmental factors (i.e., temperature, wind, cloud, rain, snow, fog, and moon phase) do not influence estimates of deer density enough to warrant cancelling a deer survey due to inclement weather.

#### Suggestions for Improvement: 

A limitation of this study is that the data was not captured at TMD training sites.  Wind, rain, and snow could also be measured in a way that better reflects the variance that these variables produce both directly, in deer movement, and indirectly, in deer density estimates.  For example, wind varies spatially and temporally. That is, wind velocity will vary drastically from one location to another and at different snapshots in time. Ideally, staff would collect wind measurements several times during a survey.  However, this is overly burdensome to staff, and thus, averaging wind measurements taken at the beginning, middle, and end of a survey would suffice.  Capturing rain and snow data could be improved by recording the data as a numerical index instead of boolean.  For example, rain and snow could be an index of 0-5, 0 being no rain/snow, and 5 being heavy rain/snow.  Staff could record rain/snow at the beginning, middle, and end and average these for the survey.  

**Figure 1**. Relationship between temperature and estimates of deer density in the Great Smoky Mountains, Cades Cove, Townsend, TN 378882.
![image](https://user-images.githubusercontent.com/95881308/212176380-c400f147-0081-4860-a83c-2cdf12100d20.png)

