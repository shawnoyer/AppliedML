# AppliedML
Wine Quality Project done in DSCI 631 Applied Machine Learning for Data Science at Drexel University. Project completed on 6/7/2024.

This is an ipynb file that pulls two datasets from Kaggle (https://www.kaggle.com/datasets/uciml/red-wine-quality-cortez-et-al-2009) corresponding to red and white variants of the Portuguese "Vinho Verde" wine.   

1. The contents of the Wine Quality ipynb file are separated into three sections: 

   Goals:
	Goal 1: Classify Wine by Sugar Content - Sweet or Dry
	Goal 2: Classify Wine by Alcohol Level - Light-Bodied, Medium-Bodied and Full-Bodied
	Goal 3: Classify Wine by Quality - Good and Bad
	Goal 4: Identify the best predictive features to predict quality of wine


   EDA, Pre Processing, Feature Engineering and Feature Selection: 
	
	Accessing the data, acquiring information about the data, cleaning the data by dropping null values, plot correlation matrix, heat map, 	histograms, box plots, statistical tests such as D'Agostino-Pearson Normality Test, handling and removing outliers, create functions to 	classify wines for each goal, improve skewness using Yeo Johnson Transformation Distribution, create new data frames with processed data, 	and determined multicollinearity.

   Machine Learning Algorithms:

	To address goals 1-3, Random Forest Classifier, Gradient Boosting Classifier, and XG Boost Classifier were used. To address goal 4, Linear 	Regression and Decision Tree Regression models were used. The data was split into Train and Test, pipelines and preprocessors were set up and 	fitted, predictions were used and cross validated results. Plotted confusion matrices, ROC Curve, Precision-Recall Curve, feature importance was 	determined,  as well as hyperparameters used to identify the best parameters and scores.

2. Stakeholders and Use

   Researchers, data scientists, and enthusiasts can use this dataset to perform various kinds of analysis, such as predictive modeling, regression    
   analysis, and classification tasks. Typical tasks include predicting the quality of the wine based on its chemical properties or understanding which 
   factors influence wine quality the most.
  
3. Relevant Information:

   The two datasets are related to red and white variants of the Portuguese "Vinho Verde" wine.
   For more details, consult: http://www.vinhoverde.pt/en/ or the reference [Cortez et al., 2009].
   Due to privacy and logistic issues, only physicochemical (inputs) and sensory (the output) variables 
   are available (e.g. there is no data about grape types, wine brand, wine selling price, etc.).

   These datasets can be viewed as classification or regression tasks.
   The classes are ordered and not balanced (e.g. there are munch more normal wines than
   excellent or poor ones). Outlier detection algorithms could be used to detect the few excellent
   or poor wines. Also, we are not sure if all input variables are relevant. So
   it could be interesting to test feature selection methods. 

4. Attribute information:

   Number of Instances: red wine - 1599; white wine - 4898.

   Input variables (based on physicochemical tests):
   1 - fixed acidity
   2 - volatile acidity
   3 - citric acid
   4 - residual sugar
   5 - chlorides
   6 - free sulfur dioxide
   7 - total sulfur dioxide
   8 - density
   9 - pH
   10 - sulphates
   11 - alcohol
   Output variable (based on sensory data): 
   12 - quality (score between 0 and 10)

5. Using the Script

   The extension of the script is .ipynb so it can be accessed and run within jupyter notebook and exported as a .py to export into any Python IDE.

6. Contributors and Contact List

   Cagla Keles - Drexel University Doctoral Student, ck976@drexel.edu

   Shawn Oyer - Drexel University Gradate Student, sbo33@drexel.edu

7. License Use

   Database Contents License (DbCL) v1.0 - 

   RIGHTS GRANTED AND CONDITIONS OF USE
   Rights granted. The Licensor grants to You a worldwide, royalty-free, non-exclusive, perpetual, irrevocable copyright license to do any act that is       	restricted by copyright over anything within the Contents, whether in the original medium or any other. These rights explicitly include commercial 	use, and do not exclude any field of endeavour. These rights include, without limitation, the right to sublicense the work.

   Conditions of Use. You must comply with the ODbL.

   Relationship to Databases and ODbL. This license does not cover any Database Rights, Database copyright, or contract over the Contents as part of the 	Database. Please see the ODbL covering the Database for more details about Your rights and obligations.

   Non-assertion of copyright over facts. The Licensor takes the position that factual information is not covered by copyright. The DbCL grants you 	permission for any information having copyright contained in the Contents.

   WARRANTIES, DISCLAIMER, AND LIMITATION OF LIABILITY
   The Contents are licensed by the Licensor “as is” and without any warranty of any kind, either express or implied, whether of title, of accuracy, of 	the presence of absence of errors, of fitness for purpose, or otherwise. Some jurisdictions do not allow the exclusion of implied warranties, so 	this exclusion may not apply to You.

   Subject to any liability that may not be excluded or limited by law, the Licensor is not liable for, and expressly excludes, all liability for loss 	or 	damage however and whenever caused to anyone by any use under this License, whether by You or by anyone else, and whether caused by any fault on 	the part of the Licensor or not. This exclusion of liability includes, but is not limited to, any special, incidental, consequential, punitive, or 	exemplary damages. This exclusion applies even if the Licensor has been advised of the possibility of such damages.

   If liability may not be excluded by law, it is limited to actual and direct financial loss to the extent it is caused by proved negligence on the 	part 	of the Licensor.

8. Sources
  Created by: Paulo Cortez (Univ. Minho), Antonio Cerdeira, Fernando Almeida, Telmo Matos and Jose Reis (CVRVV) @ 2009

  This dataset is public available for research. The details are described in [Cortez et al., 2009]. 
  Please include this citation if you plan to use this database:

  P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis. 
  Modeling wine preferences by data mining from physicochemical properties.
  In Decision Support Systems, Elsevier, 47(4):547-553. ISSN: 0167-9236.

  Available at: [@Elsevier] http://dx.doi.org/10.1016/j.dss.2009.05.016
                [Pre-press (pdf)] http://www3.dsi.uminho.pt/pcortez/winequality09.pdf
                [bib] http://www3.dsi.uminho.pt/pcortez/dss09.bib
