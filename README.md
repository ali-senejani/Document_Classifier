# <center> Document_Classifier

**Aim:**
*document_classifier.ipynb* compares the performance of the Naive Bayes classifier to a neural net for document classification after feature transformation.<br>Final results show significant increase in performance metrics when using a shallow neural net compared to a Naive Bayes classifier. 

**Data:**
The data is obtained from the **training set** of the Kaggle competition, [Coleridge Initiative - Show Us the Data](https://www.kaggle.com/c/coleridgeinitiative-show-us-the-data) and consists of published research articles (documents) and their labels, which are datasets cited by the articles. Since the public test set is limited to only 4 documents, the focus will be on the training set, containing 19,661 records. 

The aim of the competition was to create a model capable of identifying datasets cited in research papers. The inherent difficulty of this task has to do with the infinitely large number of datasets in the wild that any given article can cite, while having a limited number of datasets (labels) for training a model. 

Unlike the competition, the purpose here is to simply create a classifier on existing dataset labels and accurately classify new documents that contain one of such labels. Hence, we will evaluate the performance of a baseline classifier (Naive Bayes) to a neural net by spliting the train dataset from the competition to train, validation and test sets of our own. 

The notebook is structured as follows:
1. Data preprocessing and exploratory data analysis
3. Feature transformation using TFIDF and label encoding
2. Evaluating of Naive Bayes classifier
3. Evaluation of neural net classifier
4. Conclusion 
