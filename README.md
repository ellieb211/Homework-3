# Homework 3
Question 1
Opens github and creates this :)

Question 2
Open recommendations.csv data 
download packages
fit the model using m <- glm(RecommendationFollowed ~ Mode, recommendations, family = binomial())
make a plot
created a plot by creating a dummy variable for the RecommedationFollowed factor
Using this in order to identify the relationship between the the modality of recommendation and recommendation followed
This showed significant results for visual recommendations - not significant for auditory
Adding in another variable for the distinction material - by creating a linear model, how composite intellect and modality of recommendation can affect whether the recommendation is followed. 
fit <- lm(RecommendationFollowed ~ Mode + CompositeIntellect, data=recommendations)
This code created the new model with the added variable 

Importing face data 
must rename the "emotionally stable" variable to something else as the code would not allow the space when attempting a PCA.
emotionally stable = e_stable
Principle Components analysis
my_prin_comps <-  prcomp(~ dominant + threatening + caring + attractive + aggressive + mean + intelligent + confident + trustworthy + e_stable + responsible + sociable + weird + unhappy , faces)
creating a scree plot to visualise how the variables account for the social judgements on faces

open faces_big file
created lantent variables using faces_b <- "valence =~ trustworthy + caring + responsible + sociable 
                dominance =~ dominant + confident + aggressive + mean"
model_faces <- cfa(faces_b, faces_big)
summary(model_faces)
and viewing the output showed that trustworthy was in the wrong section. 

creating a visual model better shows this. 
This is the way of analysing this model
##visualisation model – useful to identify structure of model
##square – measure variables 
##circle – factors – latent variables not measured
##numbers – unstandardised factor regression coefficients
##double arrow – variances
##dotted lines – covariances – not a part of model prediction

