# Stack Overflow Tag Predictor
Multi-label classification problem

**<h2>Description</h2>**

Stack Overflow is the largest, most trusted online community for developers to learn, share their programming knowledge, and build their careers. It is something which every programmer use one way or another. Each month, over 50 million developers come to Stack Overflow to learn, share their knowledge, and build their careers. It features questions and answers on a wide range of topics in computer programming. The website serves as a platform for users to ask and answer questions, and, through membership and active participation, to vote questions and answers up or down and edit questions and answers in a fashion similar to a wiki or Digg. As of April 2014 Stack Overflow has over 4,000,000 registered users, and it exceeded 10,000,000 questions in late August 2015. Based on the type of tags assigned to questions, the top eight most discussed topics on the site are: Java, JavaScript, C#, PHP, Android, jQuery, Python and HTML.


**<h2>Real World / Business Objectives and Constraints</h2>**
  Predict as many tags as possible with high precision and recall.
  Incorrect tags could impact customer experience on StackOverflow.
  No strict latency constraints.
  
  
**<h2>Data Overview</h2>**

Refer: https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/data

All of the data is in 2 files: Train and Test.
Train.csv contains 4 columns: Id,Title,Body,Tags.
Test.csv contains the same columns but without the Tags, which you are to predict.
Size of Train.csv - 6.75GB
Size of Test.csv - 2GB
Number of rows in Train.csv = 6034195



**<h2>Data Field Explaination</h2>**

Dataset contains 6,034,195 rows. The columns in the table are:
Id - Unique identifier for each question
Title - The question's title
Body - The body of the question
Tags - The tags associated with the question in a space-seperated format (all lowercase, should not contain tabs '\t' or ampersands '&')

This is a multi-label classification problem (http://scikit-learn.org/stable/modules/multiclass.html)



**<h2>Performance metric</h2>**

Micro-Averaged F1-Score (Mean F Score) : The F1 score can be interpreted as a weighted average of the precision and recall, where an F1 score reaches its best value at 1 and worst score at 0. The relative contribution of precision and recall to the F1 score are equal.

In the multi-class and multi-label case, this is the weighted average of the F1 score of each class.
