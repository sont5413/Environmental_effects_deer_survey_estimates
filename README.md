#### Project Objective

The objective of this project was to determine if environmental factors influence estimates of white-tailed deer density from spotlight surveys, a standard method in estimating white-tailed deer population abundance. The results of this study are intended to improve TMD’s data accuracy and planning of annual spotlight deer surveys.

#### Methods: 

Spotlight survey data was collected by the Department of the Interior in Great Smoky Mountains National Park from 1993-2003.  The spotlight survey route was within Cades Cove, Townsend, TN 378882.  Several rows of temperature data were missing. Missing temperature data was replaced by data recorded at the Knoxville airport, which was the closest national weather service station that had data for the missing days.  The following environmental variables were recorded:
* month of the year (numerical)
* temperature (numerical)
* wind (Boolean)
* cloud cover (categorical)
* rain (Boolean)
* snow (Boolean)
* fog (Boolean)
* moon phase (categorical)

#### Results: 

The environmental factors listed above do not significantly influence estimates of deer density made from spotlight surveys. Temperature was found to be the most influential predictor from a simple linear regression model (SLR) and two optimized machine learning models (i.e., random forest and gradient boosting optimized via GridSearchCV). The R<sup>2</sup> (i.e., proportion of variance explained by the model) of the selected linear model was poor (~ 0.17). The mean absolute error (MAE) of the SLR was 7.09.  Temperature was a statistically significant predictor (p < 0.001). The selected SLR found that for every 1 degree Fahrenheit increase in temperature, there was a 0.40 acre/deer decrease in deer density.

The optimized random forest regressor and gradient boosting regressor achieved MAEs of 2.69 and 4.34, respectively.  Both of these models were a better fit to data than the SLR.  All models reported that temperature was the most influential variable. The machine learning models both reported that the variable “month” was the second most influential important feature.  


#### Management Implications: 

Environmental factors (i.e., temperature, wind, cloud, rain, snow, fog, and moon phase) do not influence estimates of deer density enough to warrant cancelling a deer survey due to inclement weather.

#### Suggestions for Improvement: 

A limitation of this study is that the data was not captured at TMD training sites. Wind, rain, and snow could also be measured in ways that better reflect the variance that these variables produce both directly, in deer movement, and indirectly, in deer density estimates. For example, wind velocity varies spatially and temporally. That is, wind velocity will vary drastically from one location to another and at different snapshots in time. Ideally, staff would collect wind measurements several times during a survey. However, this is overly burdensome to staff, and thus, averaging wind measurements taken at the beginning, middle, and end of a survey would suffice. Capturing rain and snow data could be improved by recording the data as a numerical index instead of as a Boolean variable. For example, rain and snow could be an index of 0-5, 0 being no presence of rain/snow, and 5 being heavy rain/snow. Staff could record the index of rain/snow at the beginning, middle, and end and average these three recordings to represent the rain/snow index for the survey.


**Figure 1**. Scatterplot with regression line of the relationship between temperature and deer density collected from spotlight survey data of white-tailed deer in the Great Smoky Mountains, Cades Cove, Townsend, TN 378882.
![image](https://user-images.githubusercontent.com/95881308/212176380-c400f147-0081-4860-a83c-2cdf12100d20.png)

