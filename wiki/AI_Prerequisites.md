---
layout: page
title: AI_Prerequisites
wikiPageName: AI_Prerequisites
menu: wiki
---

Helpful Prerequisites & Tools for AI Development

If you are struggling with some of the ML resources, or wish to gain further insight into the mechanics of ML, or expand your skills more generally (ex. in order to build your own models or better articulate/understand ML concepts) here is a list of some of the fundamental skills / topics that provide a good foundation. Each section starts with the most pertinent general tools/topics, then progresses into more niche subjects. Wherever possible, multiple resources are recommended for each topic, presuming various levels of math/programming experience.

# **Programming**

* **Command Line** (basic navigation, file & folder manipulation & editing comes in handy when dealing with code and data)
    * Unique to Mac / Linux / Windows OS ([Quick Command Line Tutorial that covers all 3](https://tutorial.djangogirls.org/en/intro_to_command_line/))
  
* **Python** (or other programming language that supports ML libraries - Python is by far the most popular - and you will see it in many tutorials and examples)
    * Basic Concepts: Functions, loops, conditionals, variables, lists, dictionaries, sets, etc.
        * [Harvard’s Introduction to Computer Programming with Python](https://cs50.harvard.edu/python/2022/) (Preq. for AI with Python course, 1 Semester of Material - Lectures, Notes, HW, Projects)
        * [University of Helsinki Introduction to Python Programming MOOC](https://programming-22.mooc.fi/)
          * Includes lecture videos, assignments, etc.
          * Also covers Advanced Course Materials (Semester 2)
          * **Unique**: hosts bimonthly exams to award credits through University of Helsinki (receive a certificate that can be transferred to your home institution) - for free!
        * [Ada Developers Academy Build Curriculum](https://github.com/Ada-Developers-Academy/ada-build) (Simple, 1-week Python Curriculum in Google CoLab to get you started with the basics)

## Data Visualization

### Javascript: functional programming language for web development
Applications: Data Visualization / Interaction / Web: (Useful knowledge for deploying ML in various environments - you can also build and train models completely in Javascript)

* [DNotebook](https://github.com/javascriptdata/dnotebook) (jupyternotebook like library for Javascript)
* [Danfo.js](https://danfo.jsdata.org/) (javascript Pandas-like data manipulation library)
* [P5.js](https://p5js.org) (javascript library for creative coding)
  * [ML5.js](https://ml5js.org/) (ML specific javascript library built to work with P5.js
* [D3.js](https://d3js.org/) - Javascript document manipulation library - manipulate documentation directly from data (ex. create interactive barchart that responds to changing dataset)
* [Observable](https://observablehq.com/tutorials) A javascript notebook based visualization tool  (tutorials, examples, etc.)

#### ML specific libraries for Javascript: 
* [Torch.js](https://github.com/torch-js/torch-js)(JS binding for PyTorch - allows you to run torch script inside Node.js)
* [TensorFlow.js](https://www.tensorflow.org/js)
* [ML5.js](https://ml5js.org/) (ML specific javascript library built to work with P5.js
[A Beginner's Guide to Machine Learning with ml5.js"](https://www.youtube.com/watch?v=jmznx0Q1fP0)
* [Brain.js](https://brain.js.org/#/) (Library for GPU accelerated NN in Javascript)

# **Math**

## General 
* General Math for ML Texts: (Cover Math Concepts in context of ML)
  * [Artificial Intelligence Engines: A tutorial Introduction to the Mathematics of Deep Learning](https://bookshop.org/books/artificial-intelligence-engines-a-tutorial-introduction-to-the-mathematics-of-deep-learning/9780956372819)
  * - [Probabilistic Machine Learning](https://github.com/probml/pml-book) (Free book series on Machine Learning, starting with focus on math and statistics)
  * - [MIT Mathematics for CS Online Course](https://openlearninglibrary.mit.edu/courses/course-v1:OCW+6.042J+2T2019/about)

## Algebra

### Traditional Algebra (Variables, functions, linear equations, logarithmic functions, etc)
  * [Khan Academy Algebra 1](https://www.khanacademy.org/math/algebra)  - Variables, fxns, linear eq.
  * [Khan Academy ALgebra 2](https://www.khanacademy.org/math/algebra2) - polynomials, exponents, logarithmic functions
  
### Linear Algebra (Tensors & matrix multiplication)
  * 3B1B - [Essence of Linear Algebra Series](https://www.3blue1brown.com/topics/linear-algebra)
  * [Numerical Linear ALgebra for Programmers](https://aiprobook.com/numerical-linear-algebra-for-programmers/) - part of Interactive Programming for Artificial Intelligence Series
  * Textbook: Linear Algebra Done Right: [https://linear.axler.net/](https://linear.axler.net/)
  * (After Learning LA) Introduction to Tensor Calculus: [https://www.ita.uni-heidelberg.de/~dullemond/lectures/tensor/tensor.pdf](https://www.ita.uni-heidelberg.de/~dullemond/lectures/tensor/tensor.pdf)
      * Good for giving intuition for _why_ we deal with tensors in linear algebra
  
## Calculus (Derivatives, gradients, chain rule, etc)
* 3B1B - [Essence of Calculus Video Series](https://www.3blue1brown.com/topics/calculus)
* Free beginner calculus curriculum ([https://math.mit.edu/~djk/calculus_beginners/](https://math.mit.edu/~djk/calculus_beginners/))
* [Calculus with Julia](https://jverzani.github.io/CalculusWithJuliaNotes.jl/) Learn calculus using the Julia programming language. (graphical, numerical, verbal and algebraic illustration - good for visual learners)
  * Requires knowledge of [Julia](https://julialang.org/), a fairly accessable programming language
* Advanced topics (not strictly necessary but helpful for digging)
  * Applied Category Theory
      * [https://arxiv.org/abs/2106.07032](https://arxiv.org/abs/2106.07032)
  * Graph Theory
      * [https://hci.iwr.uni-heidelberg.de/semmlgt](https://hci.iwr.uni-heidelberg.de/semmlgt)

# **Data Science**

## General


## Statistics (Mean, median, standard deviation, etc.)

### Courses
### Books
- [The Elements of Statistical Learning](https://hastie.su.domains/ElemStatLearn/) (Free Book on Data Mining, Inference, and Prediction) - ML text with Statistics Emphasis
- [Bayes Rules](https://www.bayesrulesbook.com/) - Free online book and community around introductory Baysian statistics 
- [Think Bayes](http://allendowney.github.io/ThinkBayes2/) - Free CCA book covering Bayesian statistics using computational methods (Colab Notebooks with exercises)
- [Introduction to Statistical Learning with R](https://www.statlearning.com/) - Free online ML text with emphasis on statistics concepts. Includes labs in R for each topic (potentially of interest to those already working in R)

## Data Collection & Manipulation: 
A large part of building AI models is aquiring and pre-processing data to train on. Knowing how to source, clean, and organize data is an essential skill.
  * **Libraries:** ML requires the input and processing of data, so it is helpful to be familiar with relevant libraries (Data Science programming courses will introduce you to these tools, or you can learn the libraries independently).
      * Super quick [numPy](https://colab.research.google.com/github/google/eng-edu/blob/main/ml/cc/exercises/numpy_ultraquick_tutorial.ipynb?utm_source=mlcc&utm_campaign=colab-external&utm_medium=referral&utm_content=mlcc-prework&hl=en), [Pandas](https://colab.research.google.com/github/google/eng-edu/blob/main/ml/cc/exercises/pandas_dataframe_ultraquick_tutorial.ipynb?utm_source=mlcc&utm_campaign=colab-external&utm_medium=referral&utm_content=mlcc-prework&hl=en) tutorials (2 heavily used DS libraries for Python)
      * See [Kaggle.com](http://kaggle.com) for additional data processing tutorials, longer-form tutorials
* **Data Collection**
  * Web Scraping: A technique for extracting data from websites (HTML & XML files) in bulk 
    * [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - Python web scraper library
* **GPU Acceleration & Optimization**: Learn to leverage hardware and data structures for improved training and inferrence speeds (useful when working with large data sets)


