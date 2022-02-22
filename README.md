# Machine-Learning
# University of Essex
# School of Computer Science and Electronic Engineering
# CE802 Machine Learning
# Assignment objectives
This document specifies the coursework assignment to be submitted by students taking CE802.
Aims of this assignment are: a) to learn to identify machine learning techniques appropriate for
a particular practical problem; and b) to undertake a comparative evaluation of several machine
learning procedures when applied to the specific problem.
# Assignment description
# 1. Pilot-Study Proposal
Imagine that you work as Machine Learning independent consultant, providing scientific advisory
and consulting services to companies seeking to apply data analytics to their business activities.
The manager of a large hotel chain contacts you to investigate the feasibility of using machine
learning to predict whether a new hotel opened in a given location will be profitable or not (i.e.
whether it will make a profit or a loss, regardless of the amount). The manager has access to
historical data of successful and unsuccessful hotels opened under the chain’s brand and she offers
to provide you with geographical and socio-economical data about the locations and neighbourhoods.
In the first part of your assignment, you are asked to write a detailed proposal for a pilot study
to investigate whether machine learning procedures could be used to successfully solve this problem.
Your report should discuss several aspects of the problem, including the following main points:
 the type of predictive task that must be performed (e.g., classification, regression, clustering,
rules mining, ...);
 examples of possibly informative features that you would like to be provided with (what
type of information that the company could obtain about the location is likely to be a good
predictor?);
 the learning procedure or procedures (e.g., DTs, k-NN, k-means, linear regression, Apriori,
SVMs, ...) you would choose and the reason for your choice;
 how you would evaluate the performance of your system before deploying it.
You can assume that the manager has some knowledge of machine learning and you do not need to
explain how the recommended learning method works. Simply discuss your recommendation and
back it with sound arguments and/or references.
This document should consist of approximately 500–750 words of narrative (i.e. excluding
references, pictures, and diagrams). Please report your word count on the title page. The document
must be submitted in PDF format with file name CE802_Pilot.pdf.
# 2. Comparative Study
Thanks to the convincing arguments in your pilot-study proposal, the company decides to collect
the data that you suggested and to hire you to perform the proposed study. They provide you with a
training set of historical data with features for each hotel opened in the past and a label representing
whether the hotel was profitable or not. These data are available in the CE802_P2_Data.zip archive
available from the CE802 moodle page. In this part of the assignment, you are asked to perform
the following two tasks.
a) Investigate the performance of a number of machine learning procedures on this
dataset. Using the data in the file CE802_P2_Data.csv contained in the CE802_P2_Data.zip
archive, you are required to perform a comparative study of the following machine learning procedures:
 a Decision Tree classifier;
 at least two more ML technique to predict if the hotel will make a profit.
You will notice that one of the features is missing for some of the instances. You are therefore
required to deal with the problem of missing features before you can proceed with the prediction step.
As a baseline approach you may try to discard the feature altogether and train on the remaining
features. You are then encouraged to experiment with different imputation methods.
The company uses Python internally and therefore Python with scikit-learn is the required
language and machine learning library for the problem. For this task, you are expected to submit a
Jupyter Notebook called CE802_P2_Notebook.ipynb containing the Python code used to perform
the comparative analysis and produce the results, as well as the code used to perform the predictions
described in task “b” below.
b) Prediction on a hold-out test set. An additional dataset, CE802_P2_Test.csv, is provided
inside the CE802_P2_Data.zip archive. Binary outcomes are withheld for this test set (i.e. the
“Class” column is empty). In this second task you are required to produce class predictions of
the records in the test set using one approach of your choice among those tested in task “a” (for
example the one achieving the best performance). These data must not be used other than to test
the algorithm trained on the training data.
As part of your submission you should submit a file called CE802_P2_Test_Predictions.csv
in CSV format, which must be identical to CE802_P2_Test.csv except that the missing class is
replaced with the output predictions obtained using your chosen approach. This second task will
be marked based on the prediction accuracy on the test set.
# 3. Additional Comparative Study
Thanks to the good results obtained in the comparative study, the hotel chain has deployed your
system and is obtaining good profit. Now a similar company would like to hire you to design a
similar system for them but, unlike the first system, they would like you to predict not only if a
new business will be profitable but also its annual profit.
They provide you with a training set of historical data containing features of each business
and a numerical value representing the profit (which may be positive or negative). These data are
a) Investigate the performance of a number of machine learning procedures on this
dataset. Using the data in the file CE802_P3_Data.csv contained in the CE802_P3_Data.zip
archive, you are required to perform a comparative study of the following machine learning procedures:
 Linear Regression;
 at least two more ML technique to predict the profit.
This company too uses Python internally and therefore Python with scikit-learn is the required
language and machine learning library for the problem. For this task, you are expected to submit a
Jupyter Notebook called CE802_P3_Notebook.ipynb containing the Python code used to perform
the comparative analysis and produce the results as well as the code used to perform the predictions
described in task “b” below.
b) Prediction on a hold-out test set. An additional dataset, CE802_P3_Test.csv, is provided
inside the CE802_P3_Data.zip archive. Target values are withheld for this test set (i.e. the “Target”
column is empty). In this second task you are required to produce predictions of the records in
the test set using one approach of your choice among those tested in task “a” (for example the one
achieving the best performance). These data must not be used other than to test the algorithm
trained on the training data.
As part of your submission you should submit a file called CE802_P3_Test_Predictions.csv
in CSV format, which must be identical to CE802_P3_Test.csv except that the missing “Target”
column is replaced with the output predictions obtained using your chosen approach. This second
task will be marked based on the root mean squared error on the test set.
# 4. Report on the Investigation
After conducting the studies in parts 2 and 3, you are asked to write a report containing an account
of your investigation. There should be a brief summary of the experiments performed followed by
one or more tables and/or graphs summarizing the performance of the different solutions. Any
numerical data that you include should be in a suitable graphical or tabular form. The rest of the
report should concentrate on your interpretation of the results and what they tell you about the
relative strengths and weaknesses of the alternative methods when applied to the given data.
This document should consist of approximately 750–1500 words of narrative (i.e. excluding
references, pictures, and diagrams). Please report your word count on the title page. The document
must be submitted in PDF format with file name CE802_Report.pdf.
