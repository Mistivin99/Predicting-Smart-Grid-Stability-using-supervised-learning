# Predicting-Smart-Grid-Stability-using-supervised-learning

This project assesses Electrical Grid Stability data to predict if a given combination of power system conditions would result in an unstable grid - and therefore risk causing blackouts or damaging equipment.  After brief data exploration and processing, I ran baseline models, confirmed my feature selection, then optimised the models. The best classifier scored 98.3% accuracy on held out data, while the best regressor gave an R2 score of 95.9%.

**Dataset**

The data set, available on Kaggle, has 10,000 instances and 12 attributes:
https://www.kaggle.com/datasets/sowlarn/ucis-electrical-grid-stability-simulated-data

•	p[x] (p1 to p4): power produced or consumed; p1 = abs(p2 + p3 + p4)
•	g[x] (g1 to g4): willingness of each node to adapt their consumption or production per second (gamma, proportional to price elasticity)
•	tau[x] (tau1 to tau4): how long it takes for each node to adapt their production or consumption in seconds
where p1, g1 and tau1 are related to the electricity producer; the rest are related to the electricity consumers.
There are also two target variables:
•	stab: a number representing grid stability (positive if unstable)
•	stabf: a categorical version of stab


