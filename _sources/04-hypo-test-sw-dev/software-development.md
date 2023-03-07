# Software development

Machine learning works essentially through running software on hardware. Most (if not all) of our efforts in machine learning are focused on developing software on purchased hardware. Machine learning software is no different from other software. It is written in programming languages, it is tested, it is deployed, it is maintained, and it is updated. In this section, we will discuss the software development process, which can help you create machine learning models more efficiently and professionally.

You should view software development as a process, not as a one-time event. A virtue of software is that it is relatively easy to change, particularly compared to hardware. Software development is a continuous process that involves many different stages, including planning, design, implementation, testing, deployment, and maintenance. In this section, we will discuss the software development process briefly, starting with the software development life cycle (SDLC).

## Software development life cycle

Watch the 9-minute video below for a visual explanation of the software development life cycle.

```{admonition} Video

<iframe width="700" height="394" src="https://www.youtube.com/embed/i-QyW8D3ei0?start=00" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[Software Development Life Cycle by Testaholic](https://www.youtube.com/embed/i-QyW8D3ei0?start=00), embedded according to [YouTube's Terms of Service](https://www.youtube.com/static?gl=CA&template=terms).
```

The [software development life cycle (SDLC)](https://en.wikipedia.org/wiki/Systems_development_life_cycle) is a process used by the software industry to design, develop, and test high quality software. The SDLC aims to produce a high-quality software that meets or exceeds customer expectations, reaches completion within times and cost estimates. The SDLC describes the stages from an initial feasibility study through maintenance of the completed application, and can be mapped to more general management control processes as shown in {numref}`SDLC-to-management` below.

```{figure} https://upload.wikimedia.org/wikipedia/commons/a/a2/SDLC_Phases_Related_to_Management_Controls.jpg
---
height: 350px
name: SDLC-to-management
---
How the SDLC phases are related to management controls  {cite}`SDLC2019`.
```

### Lifecycle phases

The SDLC typically includes the following key phases:

- **Inception** phase: The inception phase is the first phase of the SDLC. It is the phase in which the project is initiated with rationale, scope, and vision. It is also known as the feasibility study phase. Its purpose is to determine whether the project is feasible and to identify the project's scope. It is also used to determine whether the project should proceed to the next phase. It is also used to determine the project's scope and to identify the project's stakeholders.
- **Elaboration** phase ("Design/Details"): The elaboration phase is the second phase of the SDLC. Its purpose is to define the project's objectives and requirements. It involves both high-level analysis/design and detailed requirements.
- **Construction** phase ("Do it"): The construction phase is the third phase of the SDLC. Its purpose is to build the software. This phase is typically the longest phase of the SDLC. Software is typically built in increments, tested and integrated, each satisfying a subset of the requirements (see the [Agile software development](https://en.wikipedia.org/wiki/Agile_software_development) model below).
- **Transition** phase ("Deploy it"): The transition phase is the fourth phase of the SDLC. Its purpose is to transition the software from the development environment to the production environment. This typically involves installing the software on the production hardware, beta testing, performance tuning, training the users, and transferring the software to the operations and maintenance team.

### Software development models

There are several different SDLC models. We study three most popular ones below.

- **Waterfall model**: The waterfall model is a _linear, sequential_ approach, where progress is seen as flowing steadily downwards (like a waterfall) through the phases of Conception, Initiation, Analysis, Design, Construction, Testing, Production/Implementation and Maintenance. This is the traditional SDLC model. It is a simple model and easy to understand. However, it has several shortcomings, including the following:
  - It is not very flexible. Once a phase is completed, it cannot be revisited.
  - It is not very good at handling change. If requirements change during the project, the entire project may need to be restarted.
  - It is not very good at managing risk. If a problem is discovered late in the project, it may be too late to fix it.
  - It is not very good at managing quality. Quality is typically inspected at the end of the project, when it is too late to fix problems.
- **Agile model**: The [agile model](https://en.wikipedia.org/wiki/Agile_software_development) is an _iterative and incremental_ approach, where requirements and solutions evolve through collaboration between self-organizing, cross-functional teams. An incremental approach partitions a system into a number of components by functionality, and then builds each component in sequence. Typically, it will deliver an early release of a small, functional subsystem and then incrementally add more functionality to the system in later releases. The process is repeated iteratively to improve the overall system in each release.
- **Phased approach**: The phased approach is a hybrid of the waterfall and agile models. It is a _sequential_ approach, where progress is seen as flowing steadily downwards (like a waterfall) through the phases of Conception, Initiation, Analysis, Design, Construction, Testing, Production/Implementation and Maintenance. However, it is also an _iterative_ development in that each phase is repeated until the project is completed, where requirements and solutions evolve through collaboration between self-organizing, cross-functional teams. This will reduce cycle time, deliver software in pieces, let users have some functionality while developing the rest. It often have two or more systems in parallel: the operational/production system in use by customers, and the development system to replace the current release when it is ready.

The agile/phased model is more popular in the software industry today. It allows for changes in requirements and solutions. It is also a more collaborative approach that can involve more people in the development process more effectively. The agile model is also more suitable for machine learning projects, which are often iterative and incremental in nature.

### Good software development practices

In development software, you should plan for changes from the beginning and be aware of the cost involved. In developing machine learning software, it will be useful to follow the following good software development practices:

- Get a small subset of your dataset or a reduced version of your system to study, develop, debug, and test.
- Break down big/difficult problem into smaller/easier sub-steps (avoid black-box debugging).
- Be structured, organised, and logical throughout the development process.
- Keep good documentation of your code and your development process. Provide standard documentation, including a README file, a requirements file, and a license file. Add comments to your code to explain what it does and why it does it to facilitate and reduce the cost of software maintenance.
- Get help online (e.g. search) and keep the references.
- Make your code modular and reusable. Modularity helps manage change because modules help to isolate and localize bugs and changes. This will make it easier to maintain and update your code.
- Use version control software, such as Git, to track changes to your code. This will make it easier to maintain and update your code, as well as collaborate with others. This will be the next topic we will discuss in this section.

## GitHub for software development

[GitHub](https://en.wikipedia.org/wiki/GitHub) is a web-based hosting service for version control using [Git](https://en.wikipedia.org/wiki/Git). It is mostly used for computer code. It offers all of the distributed version control and source code management (SCM) functionality of Git as well as adding its own features. It provides access control and several collaboration features such as bug tracking, feature requests, task management, and wikis for every project. GitHub is a subsidiary of Microsoft, which acquired the company in 2018 for US$7.5 billion.

### Why use GitHub?

GitHub is a popular platform for software development. It is used by many software developers, including us, the instructors, for both teaching and research. For example, this course is hosted on GitHub. It is also used by many companies for their software development, including Google, Facebook, Microsoft, and Amazon, by many open-source projects, including the Linux kernel and the Python programming language, and by many research projects, including the [scikit-learn](https://scikit-learn.org/stable/) machine learning library and the [PyTorch](https://pytorch.org/) machine learning library.

GitHub is a good place to store your code and collaborate with others. It is also a good place to showcase your work to potential employers and learn from others. You can also use GitHub to host your website. Some employers may ask you to provide a link to your GitHub profile as part of your job application. Therefore, we strongly encourage you to [create a GitHub account](https://github.com/join) and use it for your software development.

### How to use GitHub?

Watch the 8-minute video below for a visual explanation of how to use GitHub for software development.

```{admonition} Video

<iframe width="700" height="394" src="https://www.youtube.com/embed/iv8rSLsi1xo?start=01" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[GitHub Tutorial - Beginner's Training Guide by Anson Alexander](https://www.youtube.com/embed/iv8rSLsi1xo?start=01), embedded according to [YouTube's Terms of Service](https://www.youtube.com/static?gl=CA&template=terms).

```

We recommend you to use [Visual Studio Code (VS Code)](https://code.visualstudio.com/) as your code editor, which has a [GitHub extension](https://code.visualstudio.com/docs/editor/github) to help you use GitHub. It is a free, open-source, cross-platform code editor developed by Microsoft. It is available for Windows, macOS, and Linux. It is a very popular code editor among software developers. You can also use other code editors such as [PyCharm](https://www.jetbrains.com/pycharm/), [Spyder](https://www.spyder-ide.org/), and [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/). [GitHub Desktop](https://desktop.github.com/) is a popular application dedicated to manage your GitHub repositories. You can also read the [GitHub Guides](https://guides.github.com/) for more information.

## Randomness and reproducibility

In machine learning, we often use random numbers to generate random data, shuffle data, and initialise parameters. We also use random numbers to split data into training, validation, and test sets, and to select hyperparameters. Therefore, it is important to understand how to generate random numbers and how to make your code reproducible.

### Random numbers

A random number is a number that is generated by a random process, typically is governed by a probability distribution in programming. In Python, we can use the [random](https://docs.python.org/3/library/random.html) module to generate random numbers for various distributions. Many Python libraries have their own random number generators, such as [NumPy](https://numpy.org/doc/stable/reference/random/index.html), [TensorFlow](https://www.tensorflow.org/api_docs/python/tf/random), and [PyTorch](https://pytorch.org/docs/stable/torch.html#random-number-generation).

### Random seeds for reproducibility

When there are randomness in the machine learning process, we need to set a random seed to make the results reproducible, typically at the beginning of our code. A random seed is a number used to initialize a pseudorandom number generator. It is used to generate a sequence of numbers that can be predicted/reproduced when running multiple times. In Python, we can use the [random.seed](https://docs.python.org/3/library/random.html#random.seed) function to set the random seed. We can also use the [numpy.random.seed](https://numpy.org/doc/stable/reference/random/generated/numpy.random.seed.html) function to set the random seed for NumPy. We can also use the [torch.manual_seed](https://pytorch.org/docs/stable/generated/torch.manual_seed.html) function to set the random seed for PyTorch.

For example, in [Hypothesis testing on synthetic dat](https://pykale.github.io/transparentML/04-hypo-test-sw-dev/hypothesis-testing.html#hypothesis-testing-on-synthetic-data), we used the [NumPy](https://numpy.org/doc/stable/reference/random/index.html) module to generate random numbers for the [NumPy](https://numpy.org/doc/stable/reference/random/index.html) array via `np.random.seed(2022)` so that the results are reproducible on my machine and yours. When using multiple libraries with randomness involved, you need to set the random seed for each library. You can take a look at how we set seeds for commonly used libraries in our own [PyKale](https://github.com/pykale/pykale) library [here](https://github.com/pykale/pykale/blob/main/kale/utils/seed.py).

To make your code reproducible, setting random seeds is only the most basic step. Version control software, such as Git, is also needed to track changes to your code, which is one of the reasons we recommend you to use GitHub for your software development. You can also use [Docker](https://www.docker.com/) to package your code and its dependencies into a container image, which can be used to run your code in a reproducible environment. More advanced methods include the use of [Continuous Integration (CI)](https://en.wikipedia.org/wiki/Continuous_integration) to automatically run your code and tests on a remote server every time you push your code to GitHub, which we have used for the course website as well as our own [PyKale](https://github.com/pykale/pykale) library via GitHub Actions (workflows).

## Exercises
**1**. The **SDLC elaboration phase** aims to determine whether the project is feasible and to identify the project’s scope.

       a. True

       b. False

*Compare your answer with the solution below*

   ```{toggle}
    **b. False. The **SDLC inception phase**** aims it.
   ```

**2**. **Agile model** is an **iterative** and **incremental** approach, where requirements and solutions evolve through collaboration between self-organising, cross-functional teams.

       a. True

       b. False

*Compare your answer with the solution below*

   ```{toggle}
    **a. True**
   ```

**3**. Create a **Github** profile of your own (if you don't have any) and try to upload **one** of the exercise notebooks you have **completed** in this course. **Hint**: See section [4.2.2](https://pykale.github.io/transparentML/04-hypo-test-sw-dev/software-development.html#github-for-software-development)
