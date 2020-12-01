# Team-ARK-Credit-Card-Fraud-Detection
CMPE-255-02-F20-Group-11

### Project Title: 

Comparison of Multiple Solutions for Credit Card Fraud Detection

### Project Description:

For this project, our team has decided to work on the Credit Card Fraud Detection dataset. We chose this dataset because of its complexity, relatively large size, and its relevance as a real world issue today. We plan to implement multiple classification methods to help us detect whether a transaction is genuine or fraudulent. The process will start by first implementing a pre-processing step to clean up our data set for better usability and to generate visualizations. This is due to the dataset consisting of multiple dimensions, and containing potentially informative outliers. Using the processed data, we will then tune and train our models. Ultimately we will compare our different methods against each other to draw conclusions on what processes performed best and produced the greater results in this scenario.

### Proposed Methodology/Techniques/Resources/Datasets:

The dataset was provided by the Universite Libre de Bruxelles’s Machine Learning Group to Kaggle at https://www.kaggle.com/mlg-ulb/creditcardfraud. It consists of approximately 285k entries with 31 columns detailing European credit card transactions from two days out of September 2013. The classes to be predicted on this dataset are binarily encoded with “1” representing fraudulent transactions and “0” representing all others. To obscure sensitive information from the public, most features of this dataset have been published after already undergoing PCA transformations, with only the values “Time”, and “Amount” untransformed. “Time” represents seconds from the beginning of the dataset, while “Amount” is the total amount charged during each transaction.

The dataset is interesting in that the classes are highly imbalanced, with only around 0.17% of entries falling under the “fraud” classification. Due to this aspect of the dataset, accuracy can become misleading. Therefore, we expect to use metrics such as Precision, Recall and F1 instead. We intend to look at the confusion matrix with the data as a means of visualization, with the goal of achieving a result that provides a high recall, or low false negatives meaning we maximize finding all the fraudulent cases. We will be looking into the ROC and the AUROC to better understand our models’ performance. On top of this, preprocessing techniques will need to be utilized to balance the data for model training.

As this dataset is a collection of many different card holders with the goal of classification, the main techniques to be used are those related to dimensionality reduction, classification, and clustering. While most features of this dataset have previously undergone PCA transformations, the data is still complex and could potentially benefit from further dimensionality reduction.The models we are considering to utilize and compare include decision trees, nearest-neighbor classifiers, and artificial neural networks. Within these models, we also plan on comparing results given different hyper-parameter values, ensemble learning methods, and dataflow architectures.

The primary language planned to be used in this project is Python. Some libraries we plan on utilizing include Scipy, Numpy, Pandas, Sklearn, and Tensorflow. A git repository will be set up where all members will collaborate and contribute to the code. Additional languages and libraries may be added throughout the course of the project.

### References
Andrea Dal Pozzolo, Olivier Caelen, Reid A. Johnson and Gianluca Bontempi. Calibrating Probability with Undersampling for Unbalanced Classification. In Symposium on Computational Intelligence and Data Mining (CIDM), IEEE, 2015
Dal Pozzolo, Andrea; Caelen, Olivier; Le Borgne, Yann-Ael; Waterschoot, Serge; Bontempi, Gianluca. Learned lessons in credit card fraud detection from a practitioner perspective, Expert systems with applications,41,10,4915-4928,2014, Pergamon
Dal Pozzolo, Andrea; Boracchi, Giacomo; Caelen, Olivier; Alippi, Cesare; Bontempi, Gianluca. Credit card fraud detection: a realistic modeling and a novel learning strategy, IEEE transactions on neural networks and learning systems,29,8,3784-3797,2018,IEEE
Dal Pozzolo, Andrea Adaptive Machine learning for credit card fraud detection ULB MLG PhD thesis (supervised by G. Bontempi)
Carcillo, Fabrizio; Dal Pozzolo, Andrea; Le Borgne, Yann-Aël; Caelen, Olivier; Mazzer, Yannis; Bontempi, Gianluca. Scarff: a scalable framework for streaming credit card fraud detection with Spark, Information fusion,41, 182-194,2018,Elsevier
Carcillo, Fabrizio; Le Borgne, Yann-Aël; Caelen, Olivier; Bontempi, Gianluca. Streaming active learning strategies for real-life credit card fraud detection: assessment and visualization, International Journal of Data Science and Analytics, 5,4,285-300,2018,Springer International Publishing
Bertrand Lebichot, Yann-Aël Le Borgne, Liyun He, Frederic Oblé, Gianluca Bontempi Deep-Learning Domain Adaptation Techniques for Credit Cards Fraud Detection, INNSBDDL 2019: Recent Advances in Big Data and Deep Learning, pp 78-88, 2019
Fabrizio Carcillo, Yann-Aël Le Borgne, Olivier Caelen, Frederic Oblé, Gianluca Bontempi Combining Unsupervised and Supervised Learning in Credit Card Fraud Detection Information Sciences, 2019
Machine Learning Group - ULB. “Credit Card Fraud Detection.” Credit Card Fraud Detection, Kaggle, 2016, www.kaggle.com/mlg-ulb/creditcardfraud. 
