# multivariate_descriptive_analysis
Using random forest model to generate insights into a data that can't be found using traditional EDA

# Background

Most of the times in order to get inisights from a data, the solution is doing exploratory data analysis which is mostly on a univariate level or sometimes bi variate, but this doesn't give the effect of a combination of features that could be important. One way to tackle this is to build multiple decision trees using random forest and plotting them. Each tree would give some nodes as a combination of features (f1>2 & f3<6 etc...,) which have a significant disparity in the target value. This could be interpreted as a section of the population that signifcantly vary from the overall population in terms of the target.

For the sake of this project, I've used a small dataset from kaggle which has a few features on student education and experience and the target being if the student got placed in a job.

# Method

Although it's very easy to plot these trees, they need to be interpreted manually and to get the data in a node, we need to use the conditions again. The aim of this project is to create an automated way which transforms these trees in a different way and gives two dictionaries as output where one is the dictionary of conditions and the summary of a node and the other is a dictionary of dataframes with these conditions.

Here's an example. The nodes correspond to the keys of the dictionary

![tree](https://user-images.githubusercontent.com/37741896/141938446-56be7f48-7290-428a-bfae-f8d34e3c38ed.png)

The dataframe outputs can be used for any further analysis needed.
