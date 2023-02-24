# Homework 3
 Homework 3
Question 2
Open recommendations.csv data 
download packages
fit the model using m <- glm(RecommendationFollowed ~ Mode, recommendations, family = binomial())
make a plot
Using this in order to identify the relationship between the the modality of recommendation and recommendation followed
This showed significant results for visual recommendations - not significant for auditory
Adding in another variable for the distinction material - by creating a linear model, how composite intellect and modality of recommendation can affect whether the recommendation is followed. 
fit <- lm(RecommendationFollowed ~ Mode + CompositeIntellect, data=recommendations)
This code created the new model with the added variable 

Importing face data 
must rename the "emotionally stable" variable to something else as the code would not allow the space when attempting a PCA.
emotionally stable = e_stable
