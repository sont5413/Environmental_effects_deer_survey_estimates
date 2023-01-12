#### Project Summary: 

The environmental factors below do not signiciantly influence estimates of deer density made from spotlight surveys.  Temperature was found to be the most influential predictor from a simple linear regression model (SLR) and two optimized machine learning models (i.e., random forest and gradient boosting optimzed via gridsearchcv).  The R<sup>2<sup> (i.e., proportion of variance explained by the model) of the selected linear model was poor (~ 0.10).  However, temperature was found to be a statistically significant predictor (p < 0.001).  The selected SLR found that for every 1 degree fahreheit increase in temperature, there was a 0.80 decrease in the deer density. Environmental factors: 

* month of the year (numerical)
* temperature (numerical)
* wind (boolean)
* cloud cover (categorical)
* rain (boolean)
* snow (boolean)
* fog (boolean)
* moon phase (categorical)

#### Dataset: 

This is deer spotlight survey data collected by the Department of the Interior in Great Smoky Mountains National Park from 1993-2003.

####  Results and Management Implications: 

Environmental factors (i.e., temperature, wind, cloud, rain, snow, fog, and moon phase) do not influence estimates of deer density enough to warrant cancelling a deer survey due to 

#### Suggestions for Improvement: 

A limitation of this study is that the dataset is not taken directly from TMD training sites.  Confidence in the results and implications would be higher had the data been collected at TMD's training sites.  Wind, rain, and snow could also be measured in a way that better reflects the variance that these variable produce both directly, in deer movement, and indirectly, in deer density estimates.  For example, wind varies spatially and temporally. That is, wind velocity will vary drastically from one location to another and at different snapshots in time. Ideally, staff would collect wind measurements several times during a survey.  However, this is overly burdensome to staff, and thus, averaging wind measurements taken at the beginning, middle, and end of a survey would suffice.  Capturing rain and snow data could be improved by recording the data as a numerical index instead of boolean.  For example, rain and snow could be an index of 0-5, 0 being no rain/snow, and 5 being heavy rain/snow.  Staff could record rain/snow at the beginning, middle, and end and average these for the survey.  
