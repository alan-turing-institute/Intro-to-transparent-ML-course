# Overview

**[Turing Course: An Introduction to Transparent Machine Learning](https://learn.turing.ac.uk/course/view.php?id=24)**

Welcome to [An Introduction to Transparent Machine Learning](https://www.turing.ac.uk/introduction-transparent-machine-learning), part of the [Alan Turing Institute](https://www.turing.ac.uk/)'s [online learning courses in responsible AI](https://www.turing.ac.uk/funding-call-online-learning-courses-responsible-ai). This self-paced online learning course aims to introduce essential materials on transparent machine learning for learners of diverse backgrounds to understand and apply transparent machine learning in real-world applications with confidence and trust, targeting a missing gap in the online educational space.

We recast selected contents from a popular, award-winning textbook [An Introduction to Statistical Learning with Applications in R](https://www.statlearning.com/) {cite}`james2021statistical` into the perspective of system and process transparency under the AI transparency framework in [AI in Financial Services](https://www.turing.ac.uk/sites/default/files/2021-06/ati_ai_in_financial_services_lores.pdf) report {cite}`ostmann2021ai` from the Alan Turing Institute, using Python. The chosen textbook is widely used as standard in many university courses on machine learning, written by leading academics, and explains topics in a highly accessible way. Under the chosen [AI transparency framework](https://www.turing.ac.uk/sites/default/files/2021-06/ati_ai_in_financial_services_lores.pdf), transparent machine learning systems will cover fully transparent machine learning models such as linear regression and "semi-transparent" machine learning models such as deep learning, and transparent machine learning processes will cover machine learning model evaluation and software development methodologies such as cross validation and software development life cycle.

This course is developed as [a PyKale repository](https://github.com/pykale/transparentML) for deployment as [an Alan Turing Institute repository](https://github.com/alan-turing-institute/Intro-to-transparent-ML-course/). Welcome your feedback/contribution via opening [issues](https://github.com/pykale/transparentML/issues), [discussions](https://github.com/pykale/transparentML/discussions), and/or [pull requests](https://github.com/pykale/transparentML/pulls).

Watch the 10-minute video below for a conversation on this course between [Lily Clements](https://www.linkedin.com/in/lily-clements-9788a512a/) and [Haiping Lu](https://www.linkedin.com/in/haiping-lu-4821206/).

```{admonition} Video
<iframe width="700" height="394" src="https://www.youtube.com/embed/e69-0hG0IqM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

[Conversation on Turing Course - An Introduction to Transparent Machine Learning](https://www.youtube.com/embed/e69-0hG0IqM), embedded according to [YouTube's Terms of Service](https://www.youtube.com/static?gl=CA&template=terms).
```

## Learning objectives [LOs]

By the end of the course, we expect a learner can demonstrate the ability to:

- [LO1] Understand the theoretical issues and wider context related to transparent machine learning systems and processes.
- [LO2] Understand the inner-working of a selected number of transparent machine learning algorithms with the capability of interpret the modelling process and the input-output relationships.
- [LO3] Deploy a practical implementation of transparent machine learning systems and processes in a real-world setting using Python libraries such as scikit-learn.
- [LO4] Visualise, interpret, and explain transparent machine learning systems and processes in a real-world setting to help stakeholders understand these systems and processes.
- [LO5] Gain the skills to confidently apply machine learning to your area of work, regardless of your background.

## Target audience

Learners from diverse backgrounds, preferably with knowledge and skills of basic mathematics (particularly probability and linear algebra) and Python programming for machine learning. We suggest those lacking such knowledge and skills to go through {doc}`Prerequisites <../00-prereq/overview>` to pass the quiz there first.

## Discussion forum for Q&A etc

We have a [discussion forum](https://github.com/pykale/transparentML/discussions) as our primary communication channel, e.g. for Q&A, information sharing, and discussion. We also provide a rich set of [labels](https://github.com/pykale/transparentML/labels) for you to label your posted messages so that similar messages can be easily found. Please ask questions or post information there, rather than emailing the instructors directly. This will help others to benefit from the answers and help build an engaging community. You will need a [GitHub account](https://github.com/join) to post questions. Please follow the [Code of Conduct](https://github.com/pykale/transparentML/blob/main/CODE_OF_CONDUCT.md) when using the discussion forum.

## How to go through the course

The course is designed to be self-paced and self-directed. The course materials are organised into a [Jupyter Book](https://jupyterbook.org/) consisting of 10 chapters, plus prerequisites. Each chapter has a number of sections. Each section is a self-contained unit of learning, mostly taking no more than 30 minutes to complete and ending with an exercise. Answers to exercises are provided but hidden so that you should solve the exercises before checking the solutions, in most cases. Each chapter will have a quiz for assessment. Answers for quizzes will NOT be provided. _You are advised to score at least **50%** to proceed to the next topic_.

For sections prepared in executable Jupyter notebooks, you will see a rocket icon <i class="fas fa-rocket"></i> at the top (mid-right) . For these sections, we suggest you to go through the materials in the browser (html) first and then launch (via <i class="fas fa-rocket"></i>) the corresponding Jupyter notebook (better in Colab) to run the code and complete the exercises. _Optional: You can also download the Jupyter notebooks and [run them locally on your machine](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/execute.html) after [installation](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/install.html)._

We design this course to be self-contained so that most users can complete in 40 hours. For those short of time and those having relevant knowledge and skills already, going through the materials here should be sufficient. For those lacking such knowledge and skills, those who want to go deeper, and those with more time available, we suggest you to (re)read the textbook [An Introduction to Statistical Learning](https://www.statlearning.com/) alongside this course. You can [buy the book](https://www.amazon.co.uk/Introduction-Statistical-Learning-Applications-Statistics/dp/1071614177) or read the [free online version in PDF](https://hastie.su.domains/ISLR2/ISLRv2_website.pdf).

## Course outline and structure

Besides the prerequisites, the 10 chapters can be grouped into two parts: part one covers primary topics and part two covers secondary topics.

- [Prerequisites](https://pykale.github.io/transparentML/00-prereq/overview.html): Basic mathematics and Python programming for machine learning

**Primary topics**

- [Chapter 1](https://pykale.github.io/transparentML/01-intro/overview.html): [System and Process] Introduction to machine learning and transparency
- [Chapter 2](https://pykale.github.io/transparentML/02-linear-reg/overview.html): [System] Linear regression
- [Chapter 3](https://pykale.github.io/transparentML/03-logistic-reg/overview.html): [System] Logistic regression
- [Chapter 4](https://pykale.github.io/transparentML/04-hypo-test-sw-dev/overview.html): [Process] Hypothesis testing and software development
- [Chapter 5](https://pykale.github.io/transparentML/05-cross-val-bootstrap/overview.html): [Process] Cross validation and bootstrap
<!-- and linear discriminant analysis -->

**Secondary topics**

- [Chapter 6](https://pykale.github.io/transparentML/06-ftr-select-regularise/overview.html): [Process and System] Feature selection and regularisation
- [Chapter 7](https://pykale.github.io/transparentML/07-trees-ensembles/overview.html): [System and Process] Trees and ensembles
- [Chapter 8](https://pykale.github.io/transparentML/08-nb-glm-svm/overview.html): [System] Generalised linear models and support vector machines
- [Chapter 9](https://pykale.github.io/transparentML/09-pca-clustering/overview.html): [System] Principal component analysis and $K$-means/hierarchical clustering
- [Chapter 10](https://pykale.github.io/transparentML/10-deep-cnn-rnn/overview.html): [System] Neural networks and deep learning

## Instructors and contributors

<table>
  <tbody>
    <tr>
      <td align="center"><a href="https://haipinglu.github.io/"><img src="https://raw.githubusercontent.com/haipinglu/hugo-academic/main/content/authors/haiping-lu/avatar.png" width="200px;" alt="Haiping Lu"/><br /><sub><b>Haiping Lu</b></sub></a></td>
      <td align="center"><a href="https://shuo-zhou.github.io/"><img src="https://raw.githubusercontent.com/shuo-zhou/shuo-zhou.github.io/master/assets/img/profile.png" width="200px;" alt="Shuo Zhou"/><br /><sub><b>Shuo Zhou</b></sub></a></td>
    </tr>
  </tbody>
</table>

This course is developed by [Haiping Lu](https://haipinglu.github.io/), a Professor of Machine Learning, and [Shuo Zhou](https://shuo-zhou.github.io/), an Academic Fellow in Machine Learning, both at the [Department of Computer Science](https://www.sheffield.ac.uk/dcs), [The University of Sheffield](https://www.sheffield.ac.uk/). H. Lu has developed and taught two machine learning courses [Machine Learning and Adaptive Intelligence](https://github.com/maalvarezl/MLAI) from 2018 to 2021 and [Scalable Machine Learning](https://github.com/haipinglu/ScalableML) since 2017. S. Zhou was a head teaching assistant of the [Machine Learning and Adaptive Intelligence](https://github.com/maalvarezl/MLAI) course in fall 2019 and he has been teaching the [Scalable Machine Learning](https://github.com/haipinglu/ScalableML) course since spring 2023.

[Mohammod Naimul Islam Suvon](https://github.com/Mdnaimulislam) contributed all the course exercises and quizzes. [Lawrence Schobs](https://github.com/Schobs) reviewed all teaching materials, provided detailed comments, added summaries and references, and refined the materials. After that, H. Lu and S. Zhou checked and refined the materials again for the release.

We thank valuable feedback received from [Catherine Inness](https://www.linkedin.com/in/catherineinness/), a Data Science Senior Manager at [Accenture](https://www.accenture.com/gb-en).

We welcome and recognise all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/pykale/transparentML/graphs/contributors).

## Key references

We design this course based on the following key references.

- Book
  - **The Textbook:** James G, Witten D, Hastie T, Tibshirani R., [An Introduction to Statistical Learning](https://www.statlearning.com/), Second Edition,  Springer, 2021. [PDF](https://hastie.su.domains/ISLR2/ISLRv2_website.pdf) {cite}`james2021statistical`
  - Ostmann F, Dorobantu C., [AI in Financial Services](https://www.turing.ac.uk/sites/default/files/2021-06/ati_ai_in_financial_services_lores.pdf), [Alan Turing Institute](https://www.turing.ac.uk/), 2021. {cite}`ostmann2021ai`
  - The Turing Way Community, [The Turing Way: A Handbook for Reproducible Data Science](https://the-turing-way.netlify.app/) {cite}`TheTuringWay`
- Code
  - [ISL_python: An Introduction to Statistical Learning with Applications in PYTHON](https://github.com/qx0731/Sharing_ISL_python)
  - [ISLR-python](https://github.com/JWarmenhoven/ISLR-python)
  - [python-novice-gapminder](https://github.com/swcarpentry/python-novice-gapminder/tree/gh-pages/_episodes)
- Course
  - [Scikit-learn Course](https://inria.github.io/scikit-learn-mooc/index.html)
  - [Deep Learning for Molecules & Materials](https://dmol.pub/)
  - [Coding for Economists](https://aeturrell.github.io/coding-for-economists/)
  - [MIMIC WFDB Tutorials](https://wfdb.io/mimic_wfdb_tutorials/)
  - [Jupyter Guide to Linear Algebra](https://bvanderlei.github.io/jupyter-guide-to-linear-algebra/intro.html)
  - [Machine Learning and Adaptive Intelligence](https://github.com/maalvarezl/MLAI)
  - [Scalable Machine Learning](https://github.com/haipinglu/ScalableML)

- Teaching
  - [Good practice by design](https://onlinelearning.london.ac.uk/2020/06/08/good-practice-by-design/)
  - [Planning your online module (DIY, lockdown style)](https://onlinelearning.london.ac.uk/2020/05/24/planning-your-online-module-diy-lockdown-style/)

## Acknowledgements

- This development is supported by the [Funding call for online learning courses in responsible AI](https://www.turing.ac.uk/funding-call-online-learning-courses-responsible-ai) from the [Alan Turing Institute](https://www.turing.ac.uk/).
- We have used [GitHub Copilot](https://copilot.github.com/) to generate some of the teaching materials.

## License

All content except for YouTube videos is released under the [MIT License](https://github.com/pykale/transparentML/blob/main/LICENSE). YouTube videos are embedded according to [YouTube's Terms of Service](https://www.youtube.com/static?gl=CA&template=terms).
