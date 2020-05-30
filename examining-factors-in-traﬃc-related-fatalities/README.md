# Examining Factors in Traffic Related Fatalities

## Executive Summary
Traffic accidents are a leading cause of fatalities. The goal of our project is to understand which factors lead to fatalities in order to create recommendations for legislation that can reduce traffic-related deaths. The audience of this project is U.S. state legislators. We used data from the U.S. National Highway Traffic Safety Administration (NHTSA) to determine the leading predictors of fatalities. Our data is from 2016 and consists of a random sample of ~44,000 accidents. We include predictors such as drivers' and vehicles' characteristics, weather conditions, use of safety equipment, and types of roads.

We build two models: 1) Multiple Logistic Regression with cross-validation and 2) Random Forest. In our original data set, 1.94% of observations consisted of fatalities. To achieve a balanced dataset, we used bootstrapping to oversample the minority class and undersample the majority class. Our final data set has 50% fatalities

Both of our models mostly agreed on what the most important predictors are. Among our most important findings were that the level of lighting is an important predictor of fatalities. In general, lower levels of lighting are associated with a higher probability of fatalities. One potential recommendation is to increase the level of lighting by adding more traffic lights. Another one of our key findings were that high speeds were associated with an increase in the probability of fatalities. One recommendation would be to increase the use of techniques that enforce speed limits (e.g., automated cameras that monitor speed, more patrol officers on the road). Finally, our models also indicated that a fire increases the probability of fatalities. Therefore, we recommend that legislation require every car to carry a fire extinguisher or to manufacture cars that use more fire-retardant materials. However, both of our models performed very well out-of-sample. We expect that the NHTSA also has a model that performs very well. Yet, while we believe that we know very well what predictors contribute to traffic fatalities, fatalities still occur because many predictors are uncontrollable and cannot be acted upon. For example, from our model, precipitation is one of the most important predictors to fatalities but it is impossible for us to control the weather or enact legislation that would prevent people from traveling during bad weather.

While our model performs well, we still have many limitations. For the sake of parsimony, we excluded pedestrian data, but recognize that this limits our overall findings and suggestions in this research paper. Additionally, we would like to have more data from the NHTSA on cases with fatalities. This would allow us to forego bootstrapping and analyze non-artificial data. Finally, another limitation to our methodology is that by using LASSO, we assume that sparsity exists in the data (and that a few predictors are actually important)


## Key Tools used:
* Logistic Regression with LASSO
* Random Forest

Adrian Fletcher, Michael Pearson, Jessica Nguyen 2019
