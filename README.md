# MANE 4333

## Final Exam

### Assigned: December 5, 2024

### Due: December 12, 2024

The midterm exam covers three major topics from MANE 4333: 1) k-nearest neighbors classifier, 2) Classification, and 3) Clustering. This exam will be a take-home exam. **You are to discuss the exam with no one and neither give or receive help from any other person. Any help from others will be consider academic dishonesty and will be reported.** 

The exam will be distributed through GitHub Classroom as previous homework assignments and the midterm exam have been distributed. Your repository should contain the following files: README.md (this file), Question1_data.xlsx, questionTwoData.xlsx,  QuestionThreeData.xslx, and FinalExam.ipynb.

Please complete the exam and submit before the end of the day on Thursday December 12, 2024. **No late submissions will be accepted.**

---

## Question 1. k-nearest neighbors classifier (24 points total)

The first question on the exam is related to the k-nearest neighbors classifier and the data is stored in the file Question1_data.xlsx. The dataset contains nine (9) features denoted as X<sub>1,</sub>, X<sub>2</sub>,...,X<sub>9</sub>. The column Class contains the classification for that observation with values 0 - negative and 1 - positive.

### Part a (8 points).

In cell two (code cell), use the technique presented in Week 10 and Homework 6 to select an optimal value of *k* based upon the accuracy of the training and testing datasets by investigating different values of *k*. Add the parameter random_state=1212 to the train_test_split command. This information should be displayed in a graph. 

### Part b (8 Points).

In cell three (Markdown cell), state the value of *k* selected based upon the results found in part a. What is the justification for the value of *k* selected.

### Part c (8 points).

In cell four (code cell), provide the Python code to implement a *k*-nearest neighbors classifier model using the value *k=9*. Print the accuracy for the training and test datasets. Generate text-based and graphical confusion matrices for the test dataset (normalized and non-normalized).

---

## Question 2. Classification (42 total points)

This question examines classification models and the data is stored in the file Question2_data.xlsx. The dataset contains twelve (12) features denoted as X<sub>1,</sub>, X<sub>2</sub>,...,X<sub>12</sub>. The column Class contains the classification for each observation with values of 0, 1 and 2.

**For parts requesting a graphical confustion matrix, modify plot_confusion_matrix so that the variable class_names matches values of the column Class whenever a graphical confusion matrix is requested.**

### Part a (7 points).

In cell five (code cell), enter the Python code to implement a DecisionTreeClassifier. When performing the test_train_split specify that random_state=1212. The DecisionTreeClassifier should specify random_state=1212 and all of the other parameters are the default values (blank).  The accuracy for the training and test datasets should should be displayed. Text-based and graphical confusion matrices should be displayed. Make sure to modify the Python code for the graphical confusion matrices to account for three states with values 0, 1, and 2. This part can be modelled after the Week 11 and Homework 7.

---

### Part b (7 points).

In cell six (code cell), enter the Python code to implement a GradientBoostClassifier. When performing the test_train_split specify that random_state=1212. The GradientBoostClassifier should specify random_state=1212 and all of the other parameters are the default values (blank).  The accuracy for the training and test datasets should should be displayed. Text-based and graphical confusion matrices should be displayed. Make sure to modify the Python code for the graphical confusion matrices to account for three states with values 0, 1, and 2. This part can be modelled after the Week 11 and Homework 7.

### Part c (7 points).

In cell seven (code cell), enter the Python code to implement a RandomForestClassifier. When performing the test_train_split specify that random_state=1212. The RandomForestClassifier should specify random_state=1212 and all of the other parameters are the default values (blank).  The accuracy for the training and test datasets should should be displayed. Text-based and graphical confusion matrices should be displayed. Make sure to modify the Python code for the graphical confusion matrices to account for three states with values 0, 1, and 2. This part can be modelled after the Week 11 and Homework 7.

### Part d (7 points).

In cell eight (code cell), enter the Python code to implement a RandomSearchCV for MLPClassifier. When performing the test_train_split specify that random_state=1212. Make sure the RandomSearchCV has a random_state parameter set to 1212 and the MLPClassifier has a random_state=1212.The accuracy for the training and test datasets should should be displayed. This part can be modelled after the Week 12 and Homework 8.

### Part e (7 points).

In cell nine (code cell), enter the Python code to implement a GridSearchCV for SVMClassifer with a RBF kernel. When performing the test_train_split specify that random_state=1212. The accuracy for the training and test datasets should should be displayed. This part can be modelled after the Week 12 and Homework 8.

### Part f (7 points).

In cell ten (markdown cell), complete the table for the accuracy of the training and test data sets for the models fitted in parts a-e. Select the best model and provide a justification for your choice.


---


## Question 3. Clustering (34 total points)

This question examines clustering and the data is stored in the file Question3_data.xlsx. The dataset contains seven (7) features denoted as X<sub>1</sub>, X<sub>2</sub>,...,X<sub>7</sub>. Clustering was covered in the Week 13 Jupyter Notebook in the course repository.

### Part a (7 points).

In cell eleven (code), perform an affinity_propagation analysis to determine the number of clusters for the data in Question3_data.xls. When performing affinity_propagation specify that random_state=1212. Add a print statement that displays the number of clusters suggested by affinity_propagation analysis.

### Part b (7 points).

In cell twelve (code), perform K-means clustering using the number of clusters found in part a. When performing KMeans specify that random_state=1212. Display the cluster centers and the cluster labels for each observation.

### Part c (7 points).

In cell thirteen (code), perform DBScan clustering. Print the cluster labels. Add a print statement that states the number of clusters used. Add another print statement that provides the number of outliers.

### Part d (7 Points).

In cell fourteen (code), perform HDBSCAN clustering. When performing HDBSCAN set the parameter random_state=1212. Print the cluster labels. Add a print statement that states the number of clusters used. Add another print statement that provides the number of outliers.

### Part e (6 points).

In cell fifteen (markdown), state which clustering algorithm you would recommend based upon the results found in parts b, c, and d of this problem. State the reason that you made your selection.

