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
 
TRAIN TEST SPLIT
  -using train_test_split the train data is splitted into a ratio of 80:20
  
STANDARD SCALER
  
  -using standard scaler all values are reduced to a standard scale
  
USING DIMENSIONALITY REDUCTION ALGORITHM- PRINCIPLE COMPONENT ANALYSIS (PCA) TO REDUCE DIMESIONS (FEATURES)
  
  -PCA is applied on the standardized data and 23 principle components are retrived from 23 features
 
  -then a graph of cumulative explained variance ratio and explained variance ratio for all 23 principle components is          plotted to observe which principle components carry least information and can be dropped
  
  - by observation last 4 principle components have minimum explained variance ratio thus they are dropped
  
  -using left nineteen principle components and kMeans to 
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
