#### Project Summary: 

The environmental factors below do not signiciantly influence estimates of deer density made from spotlight surveys.  Temperature was found to be the most influential predictor from a multiple linear regression model (MLR) and two machine learning models (random forest and gradient boosting).  The R2 (i.e., proportion of variance explained by the model) of the selected linear model was poor (~ 0.10).  However, temperature was found to be a statistically significant predictor (p < 0.001).  The selected MLR found that for every 1 degree fahreheit increase in temperature, there was a 0.80 decrease in the deer density. Environmental factors: 

* month of the year (numerical)
* temperature (numerical)
* wind (boolean)
* cloud cover (index)
* rain (boolean)
* snow (boolean)
* fog (boolean)
* moon phase (index)

#### Dataset: 

This is deer spotlight survey data collected by the Department of the Interior in Great Smoky Mountains National Park from 1993-2003.

####  Implications: 

Environmental factors (i.e., temperature, wind, cloud, rain, snow, fog, and moon phase) do not influence estimates of deer density enough to warrant cancelling a deer survey.  More research is needed on the influence of severe weather events (e.g., heavy rain and high wind) on estimates of deer density.  
