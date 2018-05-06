# Playing-with-Pima-Indian-Heritage-data

This is just a short description of my work flow, if you want to find hole work take a look at newPima Jupyter notebook  or html file. 

If your know about some supervised learning and want to apply you knowleadge with different classifier then this is the best data-set you can start with.

Last accouracy result :

GradientBoostingClassifier  mean accuracy:  82.485 %

SVM classifier with linear kernel  mean accuracy:  83.863 %

MLPClassifier(neural network mean accuracy:  85.153 %

RandomForestClassifier  mean accuracy:  76.593 %

Extra Trees Classifier  : 76.29 %


Recurment : 

1. python 3.6

2. numpy

3. panda

4. matplotlib

5. seaborn

6. tensorflow


Data :

We have 768 instances and the following 8 attributes:

1. Number of times pregnant (preg)

2. Plasma glucose concentration a 2 hours in an oral glucose tolerance test (plas)

3. Diastolic blood pressure in mm Hg (pres)

4. Triceps skin fold thickness in mm (skin)

5. 2-Hour serum insulin in mu U/ml (insu)

6. Body mass index measured as weight in kg/(height in m)^2 (mass)

7. Diabetes pedigree function (pedi)

8. Age in years (age)


Step :

1. Look the data carefully : In this part we see that there are so many zero or empty value in the data-set.

2. Vizualize the data : First i use some libary of matplotlib to vizualize the data next i use weka for an experiment. Weka give me more sensible result. 

3. Look number of empty or zero value in each feature. 

4. Choose the best feature that work for the data-set. Like Number of times pregnant is not a very good feature to be use. I use Weka to choose the best feature.

5. I find four feature is useful : 

              1. Age 
              
              2. BMI 
              
              3. Glucose 
              
              4. DiabetesPedigreeFunction 
              
6. Then i apply 6 different classifier on this data-set and yes i choose training data and test data differently. I use libary from scikit-learn. 

                 1. 'K nearest neighbors',
                 
                 2. 'Decision Tree Classifier',
                 
                 3. 'SVM classifier with RBF kernel',
                 
                 4. 'SVM classifier with linear kernel',
                 
                 5. 'Gaussian Naive Bayes',
                 
                 6. 'GradientBoostingClassifier
                 
                 7. MLPClassifier(neural network)

7. No, we reach just 77.407% accouracy.

8. Replace the zero or empty data with there mean value. 

9. Then again visualize the data.

10. Select 4 feautre that are useful.

11. Again Apply the classifier's. 

12. No, we are not done yet. Just 79.65 %.

13. Take the top 3 classifier that work well for the data-set.

14. Read the documention from scikit learn of those. Know about their parameter.

15. Then try diiferent combitaion of parameter, if you take a ML course you should you know how to use this wisely.

16. At last in MLP classifier we get 85% by applying 4 hidden layer and number of neuron 15,7,7,3 accordingly. 
