# foda-project-sds
Fundamentals of Data Analysis - Repo for Project 2020

#### Project Objective:

The objective of the project is to perform and explain simple linear regression using Python on the powerproduction dataset given. The goal is to accurately predict wind turbine power output from wind speed values using the data set as a basis.

The git repository will contain, at a minimum, the following items:
1. Jupyter notebook that performs simple linear regression on the data set.
2. In that notebook, an explanation of your regression and an analysis of its accuracy.
3. Standard items in a git repository such as a README.

To enhance the submission, consider comparing simple linear regression to other types of regression on this data set.

#### Contents of the repository

The contents of this repository are as follows:

1. .gitignore
2. LICENCE
3. Readme.md (this file)
4. FoDA Project 2020.ipynb
5. powerproduction.csv - powerproduction data on which the regression analysis has been based

#### Running the program

The program is contained within the Jupyter notebook 'FoDA Project 2020.ipynb' which is the main file in the repository.

To open and run the file:

* Open the file in Jupyter notebooks
* Run the 'import' modules cell first
* Key points within the notebook are the (1) observations and (2) statistical analysis performed (r, r-squared and RSME) for each the models (found after each code block for the model)  

All documentation is contained within the workbook itself and so has not been reproduced here.

#### Summary of the Notebook's content

- Introduction to regression, types of regression and exploring the dataset
- Analysis of the dataset including anomalies in the data
- Visual representation of the dataset including scatterplot and basic regression plot
- Explored various models of regression, each time tweaking the model and/or parametres to improve/enhance on the outputs/prediction from the regression model. We explored the following models:
    1. Simple Linear Regression using Scikit-Learn
    2. Lasso Regression using Scikit-Learn - Enhanced the Linear model by using the Lasso Regression
    3. Polynomial Regression using the polyfit function in numpy
    4. Polynomial Regression using the polyfit function where the training data has been cleaned by filtering out all zero power values
    5. Polynomial Regression using Scikit-Learn - Increased the polynomial degree factor to see the impact on the regression outcome
    6. Building a Customised Model for Regression of the Dataset - Built a customised model by segregating segments of the dataset around the cut-in and cut-off wind speed values and built separate sub-models for each segment. Combined the models to form one comprehensive model for a customised regression analysis
- Used the test, train function in Scikit-Learn to split the data for training and testing. Used pandas to create the training and testing data for the customised model.
- Observations for each of the regression models
- Potential improvements to the custom model and final observations

#### Limitations:

As the Notebook uses the random sampling functions  within Scikit-Learn and Pandas, the 'random_state' argument has been used to ensure that the training and testing data remains consistent in the Notebook. The random_state variable should be set to 'None' within the import module cells of the notebook if the user requires the training and testing data to vary with each running of the workbook. 