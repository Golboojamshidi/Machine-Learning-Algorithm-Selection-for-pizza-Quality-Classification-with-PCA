## Machine Learning Algorithm Selection for pizza Quality Classification with PCA

**Description:**

This repository contains my final project for INSE6220, where I performed Principal Component Analysis (PCA) and applied machine learning techniques to classify pizza quality based on a gradient dataset. This project serves as my portfolio to showcase my data analysis skills and ability to derive meaningful insights for decision-making.

**Table of Contents:**

- Project Overview
- Dataset
- Methods
- Results
- How to Use

**Project Overview:**

In this project, I conducted an in-depth analysis of a pizza quality dataset using Principal Component Analysis (PCA) and machine learning. This repository represents my final project for INSE6220 course (Advance Statistic Analysis), which centers around the exploration of machine learning algorithms to determine the most suitable model for pizza quality classification. The primary objective is to evaluate and compare various machine learning algorithms to ascertain which one performs optimally on the given pizza gradient dataset. The project serves as a tool for understanding the process of selecting the best ML algorithm for specific datasets and is equipped with analysis tools, including decision boundary plots, Quadratic Discriminant Analysis, Confusion Matrix, and ROC Curve.



**Dataset:**

The dataset at the core of this project is the "Pizza Ingredient Analysis Dataset." It has been carefully curated to investigate the effects of various key components, particularly fat, salt, and sodium content, on the composition and characteristics of pizza. This comprehensive dataset offers detailed measurements and attributes related to these critical factors, shedding light on how alterations in fat, salt, or sodium levels can influence the overall composition, taste, and nutritional profile of pizza. It serves as a fundamental resource for discerning the impact of these ingredients on pizza quality and healthiness, providing insights for optimizing the nutritional value and flavor of pizza creations. 

**These components are as below:**

- mois – The amount of water in the sample per 100 grammes.
- prot — The amount of protein in the sample per 100 grammes.
- fat — The amount of fat in the sample per 100 grammes. ash — The amount of ash in the sample per 100 grammes.
- sodium — The amount of sodium in 100 grammes of sample.

**Methods:**

PCA (Principal Component Analysis): I applied PCA to reduce the dimensionality of the dataset and extract the most important features.
Machine Learning Techniques: I employed machine learning algorithms such as Naïve Bayes, Extratrees classifier, and Quadratic discriminant for pizza quality classification.


To investigate the effects of PCA on Pizza’s dataset, The classification algorithms are applied to the original dataset. in addition to a PCA-applied dataset with three PCAs components. Python's PyCaret library is used for classification. The original dataset is divided into train and test sets with 70% and 30%, respectively.
There are many factors to evaluate and analyse the performance of each model, such as accuracy, precision, recall, AUC, ROC, confusion matrix, and so on. Precision measures the fraction of positive predictions, and recall measures the fraction of positives detected for each class.




**Results:**

The project's findings reveal important insights into the performance of various classification models when applied to the dataset. Before applying Principal Component Analysis (PCA), the best classification models were found to be Light Gradient Boosting Machine, Random Forest Classifier, and Extra Tree Classifier. However, after dimensionality reduction, the landscape shifted, and the best models became Naive Bayes, Extra Tree Classifier, and Quadratic Discriminant Analysis.

Notably, the reduction in dataset dimensions led to a decrease in classifier performance, as indicated by accuracy scores. Light Gradient Boosting Machine and Random Forest Classifier exhibited a reduction in accuracy of 4% and 2%, respectively, when compared to their performance on the original dataset. Strikingly, the best model for the reduced dimension data, Naive Bayes, showed a 2% lower accuracy rate than the best model for the original data, Light Gradient Boosting Machine.

To identify the possible reasons why Naive Bayes outperformed other models on the reduced dimension data, further analysis is needed. It may be attributed to the fact that Naive Bayes is well-suited to situations where variables are conditionally independent, which can be the case in lower-dimensional datasets. Additionally, the specific characteristics of the dataset, such as the nature of the features and their distributions, may favor the Naive Bayes algorithm's approach to classification.

Understanding the interplay between dataset characteristics, dimensionality reduction, and algorithm performance is crucial for making informed decisions when choosing a machine learning model for a given dataset. Further exploration and experimentation may provide deeper insights into the factors contributing to the observed model performance changes.

