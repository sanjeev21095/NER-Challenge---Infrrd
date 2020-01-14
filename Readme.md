# The challenge question
The problem is an Entity Recognition problem. You have to use python and any relevant libraries to solve this, as long as you understand underlying assumptions and methods (at least on a high level) being used. The preferred solution would include a jupyter notebook with all your analysis(EDA on dataset is recommended) and experiments accompanying the submission file.

The data is annotated for named entities:
1.	Person
2.	Location
3.	Group
4.	Creative work
5.	Corporation
6.	Product

Input:
[train.txt](https://github.com/sanjeev21095/NER-Challenge---Infrrd/blob/master/train.txt)
[test.txt](https://github.com/sanjeev21095/NER-Challenge---Infrrd/blob/master/test.txt)

Output:
submission.txt

You should train your model(s) on train.txt and compute the most probable entity label on data from test.txt. Evaluation of the model will be done on the test labels (which are not provided to you). The submission file should have Entity and corresponding label separated by a tab(\t).

Please submit a well-documented jupyter notebook containing all your analysis, solution and experiments (if any) along with the submission file. Also note down all the approaches you can think of, its advantage and disadvantages/limitations.  

Bonus Points: If you can give confidence score of a prediction along with entity predicted it would be great. 0 being - not confident, 1 being - very confident. 

# My solution
In any text document, there are particular terms that represent specific entities that are more informative and have a unique context. These entities are known as named entities , which more specifically refer to terms that represent real-world objects like people, places, organizations, and so on, which are often denoted by proper names. A naive approach could be to find these by looking at the noun phrases in text documents. Named entity recognition (NER) , also known as entity chunking/extraction , is a popular technique used in information extraction to identify and segment the named entities and classify or categorize them under various predefined classes.

[Overview of implementation](https://github.com/sanjeev21095/NER-Challenge---Infrrd/blob/master/Infrrd%20Machine%20Learning%20Assignment.ipynb):
1. Data Exploration
2. Simple classifiers - Perceptron, SGD Classifier, Multinomial Naive bayes
3. Character based LSTM
4. ELMO based residual LSTM
5. Bonus question - Confidence score for predictions
