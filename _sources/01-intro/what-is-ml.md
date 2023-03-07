# What is machine learning?

## Human learning

Learning is familiar to humans (and animals), as a continuous process that starts from birth and continues throughout life. A human child (and adult) learns new things, acquires new skills, and improves existing skills to survive and thrive in the surrounding world. A child's brain and senses perceive the facts of their surroundings to gradually learn the hidden patterns of life that help the child to craft logical rules to identify learnt patterns and predict future events.

Learning is a process of acquiring new knowledge, skills, and behaviors. Learning can be divided into two categories: **acquisition** and **performance**. Acquisition is the process of acquiring new knowledge, skills, and behaviors. Performance is the process of using the acquired knowledge, skills, and behaviors to achieve a goal. Learning can be defined as a change in behavior or knowledge that results from experience. We learn from our experiences and we learn from others. For example, we learn to walk by watching others walk, we learn to speak by listening to others speak, we learn to drive by watching others drive, and we learn to cook by watching others cook.

You may have already known, since you are here, that machines can also learn from their own experiences (and from others!). That is the subject of this course.

## A definition of machine learning

> Machine learning learns a model from data.

Machine learning takes **data** as **input** to learn a **model**, a mathematical representation of the data. This learning process is called the **training** phase and the data used in training is called the **training data**. After training, the learnt model can take new data, the **test data**, as input to generate **output** for making predictions on the test data or for exploring/explaining the test data, which is the **test** phase.

The above definition is the one we will use in this course for clarity, loosely inspired by how the human brain learns certain things based on the data it perceives from the outside world. From this definition, we can see machine learning as a set of **software** tools for **modelling** and **understanding** complex **datasets**. You may find various definitions of machine learning elsewhere. For example, machine learning, from a systems perspective, is defined as the creation of automated systems that can learn hidden patterns from data to aid in making intelligent decisions.


## AI, machine learning, and deep learning

Besides machine learning (ML), you may have also heard about artificial intelligence (AI), deep learning, and data science. Some use these terms interchangeably, but they are not the same, as shown in the figure below.

```{figure} https://github.com/microsoft/ML-For-Beginners/raw/main/1-Introduction/1-intro-to-ML/images/ai-ml-ds.png
---
height: 250px
name: fig-ai-ml-ds
---
The relationships between AI, ML, deep learning, and data science, by [Jen Looper](https://twitter.com/jenlooper) adapted from [stackexchange](https://softwareengineering.stackexchange.com/questions/366996/distinction-between-ai-ml-neural-networks-deep-learning-and-data-mining).
```

**AI** is a broad field of study that aims to create intelligent machines that can perform tasks that normally require human intelligence. There are multiple ways to achieve AI, and machine learning is one of them. As defined above, machine learning is a subfield of AI that machines acquire their experiences from data, in the form of a mathematical model. There are multiple ways of machine learning, and deep learning is one of them. **Deep learning** is a subfield of machine learning that uses deep neural networks (i.e. many layers) to learn from data. **Data science** is a broad field of study that uses scientific methods, processes, algorithms, and systems to extract knowledge and insights from data, not necessarily in the form of a mathematical model as machine learning does.

## A motivating example

Let us assume we are a consultant firm hired by a client to investigate the association between advertising and sales of a product. The [Advertising dataset](https://github.com/pykale/transparentML/blob/main/data/Advertising.csv) consists of the sales of the product in 200 different markets, and advertising budgets for the product in each of those markets for three different media: TV, radio, and newspaper. You can click the link above to view the dataset.

Our goal is to develop an accurate model that can be used to predict sales on the basis of the three media budgets so that our client can increase sales by adjusting their limited advertising budget. In this setting, the advertising budgets are input variables or _features_ while sales is an output variable or _target_.

Denote the three features as $x_1$ for TV, $x_2$ for radio, and $x_3$ for newspaper, and the target as $y$ for sales (e.g. quantity). Collectively, we denote the features as $\mathbf{x}= [x_1, x_2, x_3]^\top$ as a column vector. We can use the [dataset](https://github.com/pykale/transparentML/blob/main/data/Advertising.csv) to learn a model that can predict the sales $y$ based on the advertising budgets $\mathbf{x}$: $y = f(\mathbf{x})$.

The function $f$ is called the **model** or **predictive function**. The model $f$ is learnt from the data, which is called the **training data**. The training data consists of the features $\mathbf{x}$ and the target $y$ for each sample. In this case, the training data is a table with 200 rows and 4 columns, where each row is a sample and each column is a feature or a target. The first three columns are the features and the last column is the target.

## Exercises

**1**. Deep Learning is a **subfield** of AI.

       a. True

       b. False

*Compare your answer with the solution below*
   ```{toggle}
    **a. True. Deep learning is a branch of AI that specialises in deep neural networks.**
   ```

**2**. We collected a set of data on the top $5000$ firms in the US. For each firm, we record **profit**, **number of employees**, **industry**, and the **CEO's salary**. We want to predict the CEO's salary.

    a. What are the features here?

*Compare your answer with the solution below*

   ```{toggle}
    **profit, number of employees, and industry**
   ```
    b. What is the target variable?

*Compare your answer with the solution below*

   ```{toggle}
    **CEO's salary as we want to predict it**
   ```
