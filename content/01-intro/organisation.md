# Organisation

## The rest of the course

The rest of this course is organised into nine chapters, with appendices at the end. Each chapter will focus on either the system or the process.

We have seven chapters on ML systems, which are: [Chapter 2 on linear regression](https://pykale.github.io/transparentML/02-linear-reg/overview.html), [Chapter 3 on logistic regression and and linear discriminant analysis](https://pykale.github.io/transparentML/03-logistic-reg/overview.html), [Chapter 6 on feature selection and regularisation](https://pykale.github.io/transparentML/06-ftr-select-regularise/overview.html), [Chapter 7 on trees and ensembles](https://pykale.github.io/transparentML/07-trees-ensembles/overview.html), [Chapter 8 on generalised linear models and support vector machines](https://pykale.github.io/transparentML/08-nb-glm-svm/overview.html), [Chapter 9 on principal component analysis and $K$-means/hierarchical clustering](https://pykale.github.io/transparentML/09-pca-clustering/overview.html), and [Chapter 10 on neural networks and deep learning, including convolutional and recurrent neural networks (CNNs and RNNs)](https://pykale.github.io/transparentML/10-deep-cnn-rnn/overview.html). These chapters will cover the system side of ML. Real-world applications will be used to illustrate the concepts and techniques.

We have two chapters on ML processes, which are: [Chapter 4 on hypothesis testing and software development](https://pykale.github.io/transparentML/04-hypo-test-sw-dev/overview.html), and [Chapter 5 on cross validation and bootstrap](https://pykale.github.io/transparentML/05-cross-val-bootstrap/overview.html). These chapters will cover the process side of ML, including leave-one-out/k-fold cross validation,bootstrap, types of errors, significance of results, and the software development life cycle on GitHub.

## Real-world datasets used

In this course, we will use real-world datasets to introduce machine learning from the perspective of AI transparency. We will use the following datasets from the textbook. You can click on the name of the dataset to see the actual data.

```{list-table} Datasets used in this course, from the textbook (to refine)
:header-rows: 1
:widths: "auto"
:name: datasets-table
* - Name
  - Data provided
  - Machine learning problem
* - [Advertising](https://github.com/pykale/transparentML/blob/main/data/Advertising.csv)
  - Sales, TV, radio, newspaper
  - Predict sales based on TV, radio, and newspaper advertising
* - [Auto](https://github.com/pykale/transparentML/blob/main/data/Auto.csv)
  - Gas mileage, horsepower, and other information for cars.
  - Predict gas mileage for a car.
* - [Bikeshare](https://github.com/pykale/transparentML/blob/main/data/Bikeshare.csv)
  - Hourly usage of a bike sharing program in Washington, DC.
  - Predict the number of bikes rented per hour.
* - [Boston](https://github.com/pykale/transparentML/blob/main/data/Boston.csv)
  - Housing values and other information about Boston census tracts.
  - Predict the median value of a house.
* - [BrainCancer](https://github.com/pykale/transparentML/blob/main/data/BrainCancer.csv)
  - Survival times for patients diagnosed with brain cancer.
  - Predict the survival time for a patient.
* - [Caravan](https://github.com/pykale/transparentML/blob/main/data/Caravan.csv)
  - Information about individuals offered caravan insurance.
  - Predict whether an individual will buy caravan insurance.
* - [Carseats](https://github.com/pykale/transparentML/blob/main/data/Carseats.csv)
  - Information about car seat sales in 400 stores.
  - Predict the sales of a car seat.
* - [College](https://github.com/pykale/transparentML/blob/main/data/College.csv)
  - Demographic characteristics, tuition, and more for USA colleges.
  - Predict the number of applications received by a college.
* - [Credit](https://github.com/pykale/transparentML/blob/main/data/Credit.csv)
  - Information about credit card debt for 10,000 customers.
  - Predict the amount of credit card debt for a customer.
* - [Default](https://github.com/pykale/transparentML/blob/main/data/Default.csv)
  - Customer default records for a credit card company.
  - Predict whether a customer will default on a credit card payment.
* - [Fund](https://github.com/pykale/transparentML/blob/main/data/Fund.csv)
  - Returns of 2,000 hedge fund managers over 50 months.
  - Predict the returns of a hedge fund manager.
* - [Heart](https://github.com/pykale/transparentML/blob/main/data/Heart.csv)
  - Information about heart disease for 303 patients.
  - Predict whether a patient has heart disease.
* - [Hitters](https://github.com/pykale/transparentML/blob/main/data/Hitters.csv)
  - Records and salaries for baseball players.
  - Predict the salary of a baseball player.
* - [Iris](https://github.com/pykale/transparentML/blob/main/data/Iris.csv)
  - Measurements of 150 iris flowers.
  - Predict the species of an iris flower.
* - [Khan](https://github.com/pykale/transparentML/blob/main/data/Khan.json)
  - Gene expression measurements for four cancer types.
  - Predict the cancer type for a patient.
* - [NCI60](https://github.com/pykale/transparentML/blob/main/data/NCI60_data.csv)
  - Gene expression measurements for 64 cancer cell lines.
  - Find clusters or groups among the cell lines for personalised treatment.
* - [OJ](https://github.com/pykale/transparentML/blob/main/data/OJ.csv)
  - Sales information for Citrus Hill and Minute Maid orange juice.
  - Predict the sales of orange juice.
* - [Portfolio](https://github.com/pykale/transparentML/blob/main/data/Portfolio.csv)
  - Past values of financial assets, for use in portfolio allocation.
  - Predict the value of a financial asset.
* - [Publication](https://github.com/pykale/transparentML/blob/main/data/Publication.csv)
  - Time to publication for 244 clinical trials.
  - Predict the time to publication for a clinical trial.
* - [Smarket](https://github.com/pykale/transparentML/blob/main/data/Smarket.csv)
  - Daily percentage returns for S&P 500 over a 5-year period.
  - Predict whether the stock index with increase or decrease.
* - [USArrests](https://github.com/pykale/transparentML/blob/main/data/USArrests.csv)
  - Crime statistics per 100,000 residents in 50 states of USA.
  - Predict the crime rate in a state.
* - [Wage](https://github.com/pykale/transparentML/blob/main/data/Wage.csv)
  - Income survey data for men in central Atlantic region of USA.
  - Predict the income of men
* - [Weekly](https://github.com/pykale/transparentML/blob/main/data/Weekly.csv)
  - 1,089 weekly stock market returns for 21 years.
  - Predict the stock market return in a week
```
<!-- * - [NYSE](https://github.com/pykale/transparentML/blob/main/data/.csv)
  - Returns, volatility, and volume for the New York Stock Exchange.
  - Predict the returns of a stock. -->

The above datasets show the diverse range of problems that machine learning can solve, which shows only the tip of the iceberg actually. Applications of machine learning are everywhere, from healthcare to finance, from manufacturing to agriculture, from transportation to education, and so on. The datasets used in this course are from the textbook, which is a good starting point for learning about machine learning. However, you can also find many other datasets online, such as [Kaggle](https://www.kaggle.com/datasets), [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php), [OpenML](https://www.openml.org/), [Google Dataset Search](https://datasetsearch.research.google.com/), and so on.

## Machine learning models

This course focuses on machine learning models (or methods) that are most widely used in practice, while NOT aiming to be exhaustive in covering all the models. The following table shows the machine learning models that we will cover in this course.

```{list-table} Machine learning models/methods
:header-rows: 1
:widths: "auto"
:name: mlmethods-table
* - Method
  - Description
  - Example
* - **Linear regression**
  - A linear model for regression.
  - Predicting the price of a house.
* - **Logistic regression**
  - A linear model for classification.
  - Predicting whether a customer will default on a credit card payment.
* - **Support vector machine**
  - A kernel-based model for classification.
  - Predicting whether a customer will default on a credit card payment.
* - **Decision tree**
  - A nonlinear model for classification and regression.
  - Predicting whether a customer will default on a credit card payment.
* - **Random forest**
  - An ensemble of decision trees for classification and regression.
  - Predicting whether a customer will default on a credit card payment.
* - **Neural network**
  - A nonlinear model for classification and regression.
  - Predicting whether a customer will default on a credit card payment.
* - **$K$-means**
  - A clustering model.
  - Finding groups of similar customers.
* - **Principal component analysis**
  - A dimensionality reduction model.
  - Finding the most important features of a dataset.
```

No single model will perform well in all possible scenarios. Therefore, it is important to understand the assumptions and trade-offs of each model so that you can choose the right model for a given problem.

## Exercises

**1**. Choose **three or more** datasets of your interest from {numref}`datasets-table`. Click on the name of each chosen dataset to explore and get a sense of the data. You may not be able to get a beautiful view or a view at all for those larger ones. Write down the possible machine learning problems using terminology in {numref}`mlproblems-table` that can be solved using each of your chosen dataset.

*Compare your answer with the solution below*

   ```{toggle}

   |    Dataset    |   Machine learning problems |
   | :------------ | -------------: |
   |        Advertising      |        Regression       |
   |     Auto     |      Regression     |
   |        Bikeshare      |        Regression       |
   |     Boston     |      Regression     |
   |        BrainCancer      |        Regression      |
   |     Caravan     |      Classification      |
   |        Carseats      |        Regression       |
   |     College     |        Regression    |
   |        Credit      |        Regression       |
   |     Default     |      Classification      |
   |        Fund      |        Regression       |
   |     Hitters     |      Regression      |
   |        Iris      |        Classfication       |
   |     Khan     |      Classification     |
   |        NCI60      |       Clustering        |
   |     OJ     |      Regression      |
   |        Portfolio      |       Regression        |
   |        Publication      |        Regression       |
   |     Smarket     |      Classification      |
   |        USArrests      |        Clustering       |
   |     Wage     |      Regression     |
   |        Weekly      |        Classification       |

   ```
