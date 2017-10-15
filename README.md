# DSG-IITR-PROJECT
MUSHROOM CLASSIFICATION PROBLEM

PROBLEM STATEMENT
Tof gilled mushrooms in the Aghe dataset includes descriptions of hypothetical samples corresponding to 23 species aricus and Lepiota Family Mushroom drawn from The Audubon Society Field Guide to North American Mushrooms (1981). Each species is identified as definitely edible, definitely poisonous, or of unknown edibility and not recommended. This latter class was combined with the poisonous one. The aim of this problem is to identify the poisonous and edible class. 

SOLUTION

1.After importing given data, its analysis is done by plotting various plots and checking for discrepencies.
 
  -weight feature had 51 zero entries which was replaced by its mean (approx 33)
  
  -veil-type feature had just one value and thus it was not usefull in training model thus it was removed
  
  PLOTS
  
  -regression graph between weight radius
  
  -count plot for mushroom cap color
  
  -count plot for mushroom cap color comparing quantities of edible and poisonous mushrooms of a given cap color
  
  -count plot for mushroom odor
  
  -count plot for mushroom odor comparing quantities of edible and poisonous mushrooms of a given odor
  
  -single pie chart showing mushroom poulation type percentage
  
  -double pie chart showing mushroom population type percentage and mushroom class (edible and poisionous) percentage in each      population type
  
  -single pie chart showing mushroom habitat type percentage
  
  -double pie chart showing mushroom habitat type percentage and mushroom class (edible and poisionous) percentage in each      habitat type
  
ENCODING THE OBJECT VALUES OF FEATURES TO NUMERICAL VALUES
  
  -label encoder is imported from sklearn. preprocessing and train data is encoded
  
HEAT MAP
  
  - a heatmap is plotted on the correlation matrix of features
 
SEPARATING FEATURES AND CLASS AS X & Y RESPECTIVELY
  
STANDARD SCALER
  
  -using standard scaler all values are reduced to a standard scale
  
USING DIMENSIONALITY REDUCTION ALGORITHM- PRINCIPLE COMPONENT ANALYSIS (PCA) TO REDUCE DIMESIONS (FEATURES)
  
  -PCA is applied on the standardized data and 23 principle components are retrived from 23 features
 
  -then a graph of cumulative explained variance ratio and explained variance ratio for all 23 principle components is          plotted to observe which principle components carry least information and can be dropped
  
  - by observation last 4 principle components have minimum explained variance ratio thus they are dropped
  
  -using first nineteen principle components and kMeans to find clusters on the 19 dimensional data
  
  -plotting the clusters on 2-D pairplots using combinations of first three principle componenents( 0 & 1, 1 & 2, 0 & 2)
 
 
  TRAIN TEST SPLIT
  -using train_test_split, the train data is splitted into a ratio of 80:20 for trainig and testing the classification model
  
  FOLLOWING MODELS ARE IMPORTED AND TRAINED ON TRAIN DATA(80% OF X) AND TESTED ON TEST DATA(20% 0F X):
  
  -LOGISTIC REGRESSION
  
  -LINEAR SVC
  
  -RANDOM FOREST CLASSIFIER
  
  -K NEIGHBOURS CLASSIFIER
  
  -GAUSSIAN NB
  
  -PERCEPTRON
  
  -SDG CLASSIFIER
  
  -DESIGN TREE CLASSIFIER
  
 COMPARING THE ACCURACIES OF THE MODELS SVC AND DECISION TREE PERFORMS BEST ON BOTH THE TRAIN AND TEST DATA AND THUS SELECTED FOR THE CLASSIFICATION PROBLEM
 
 IMPORTING THE DATA TO BE PREDICTED(AS Test) THEN
 
 -Test data is analyesd by plotting pie charts and descrbing radius and weight features
 -veil-type feature is removed
 -Test data is encoded to numerical values and reduced to standard scale
 -Test data is predicted using SVC and decision tree
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
