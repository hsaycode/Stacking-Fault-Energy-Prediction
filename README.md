# Stacking Fault Energy-Prediction

## Objective:
1. To predict the Gibbs Free Energy differences between FCC and HCP phases in high-entropy alloys and further the Stacking Fault Energy based on ThermoCalc data. By determining the SFE, we can estimate deformation mechanisms in FCC metals and alloys. The activation of phenomena like transformation-induced plasticity, twinning, and dislocation gliding depends on the SFE values, which are further useful in developing new materials and alloys with specific properties.
2. To establish a relationship between the ThermoCalc calculated Gibbs free energy and the composition calculated Gibbs free energy.

## Approach and Results: 
Analysed 3000+ compositions establishing quantitative and qualitative relationships between different properties and compositions.
Visualised the relationships using scatter plots, heat maps, and Pearson Co-relation Co-efficient Matrix to decode relationships.


Designed a feature selection pipeline to identify the top 10 features from 35+ features using:
1. High correlation and low variance filters
2. Genetic algorithms
3. Random Forest, Decision Trees. and Gradient Boosting Regressor.
4. Bidirectional Wrapper methods

Conducted a SHAP analysis to understand the weightage of features of the property they are predicting. Thus, getting an insight into the connections the model develops in the black box.


Trained, validated, tested and compared mean squared error, mean absolute error, and R2 score of ANNs, Random Forest, Decision Trees, Gradient Boosting , Extra Trees Regressor, Elastic Nets.

Fine-tuned parameters of the models using GridSearchCV to achieve a maximum R2 score of 0.96 on an Extra Trees Regressor.

Developed a phase prediction model using literature data to classify the phases of the composition data from thermoCalc into BCC, FCC, IM and BCC+FCC.

Trained, validated, tested and compared accuracy scores of ANNs, Random Forest, Decision Trees, Gradient Boosting, Extra Trees Classifiers, and Elastic Nets.

Fine-tuned parameters of the models using GridSearchCV to achieve a maximum accuracy score of 80% on a gradient-boosting classifier.
