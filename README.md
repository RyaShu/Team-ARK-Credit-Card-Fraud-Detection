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
