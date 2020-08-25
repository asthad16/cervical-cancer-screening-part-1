# cervical-cancer-screening-part-1
ABSTRACT
Across the world cervical cancer is reported as a serious life-threatening disease in women despite of the fact that various treatment programs are available. Globally, mortality rate of cervical cancer is high and it can curb only through effective screening, early diagnosis and organizing awareness campaigns and treatment programs. We have used the Dataset of 858 patients containing 32 attributes from the UCI repository. The proposed work presents the application of diverse classification techniques on the available dataset. 

METHODOLOGY AND EXPERIMENTS
Approach involves pre-processing, classification process and the decision-making through predictive analysis. 
A.	Data Pre-processing
          In Data pre-processing, standard measurements such as median (used for categorical attributes), mean (used for numerical values) are used to treat the missing value from the dataset. Here we have two feature that have the missing value of around 92%, that two features are STD (Time since last diagnosis) and STD (Time since first diagnosis). In order to make results more accurate these features have been removed from data-set.

B.	Data Correlation
          The dataset has thirty attributes after data pre-processing and there are chances that some of them are correlated.To analyze the correlation of the variables with each other and heat-map is plotted.
Following observations were made: 
•	Age is highly correlated with no. of pregnancies and moderately correlated with IUD (Intrauterine Device), hormonal contraceptives and first sexual intercourse.
•	Dx: Cancer and Dx: HPV are highly correlated.
•	Smoking and no. of sexual partners are moderately correlated.
•	The various STD’S included in the study proposed show significant correlation with each other.

C.	Feature Selection 
      Feature importance was applied to find the most useful features that can be used for model training.Out of twenty-nine features, Age of the person, when first sexual act happened, total number of pregnancies, partners with whom person was sexually active, Smokes, Hormonal Contraceptives and IUD are identified as the most important attributes.  

D.	Model Selection
      Analysis of different Machine Learning models to predict the best one to detect if one is at a risk of having cervical cancer. The models used for predictive analysis are as follows listed below:

MODEL	SVM	GNB	LR	DT	KNN
				GINI	ENTROPY	
ACCURACY	93.604	9.883	93.023	93.604	92.441	93.604
ACCURACY WITH UNDERSAMPLING	14.534	84.302	71.511	43.023	51.744	63.372
ACCURACY WITH OVERSAMPLING	13.372	9.883	82.588	46.511	76.511	80.2325
AUC_ROC	0.5	0.433	0.496	0.5	0.61	0.5
ROC_AUC	0.536	0.547	0.553	0.61	0.51	0.5728

E. Results
•	Decision Tree and  K-Nearest Neighbor give highest accuracy of around 93%. 
•	The Decision Tree gives better accuracy with Gini index used as statistical measure of distribution than Entropy.





