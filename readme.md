If the field of ML was Doc Brown, this introduction to machine learning tutorial is Marty McFly. 

You'll not be able to invent time travel, but you'll be able to stumble and fall all the way to saving the day. 

# References

- This [http://ciml.info/dl/v0_9/ciml-v0_9-all.pdf], 
- This [https://www.ics.uci.edu/~welling/teaching/ICS273Afall11/IntroMLBook.pdf], 
-  and this [http://learnds.com/]

# Is there a Glossary?

- Helpful: http://alumni.media.mit.edu/~tpminka/statlearn/glossary/
- Another: https://www.analyticsvidhya.com/glossary-of-common-statistics-and-machine-learning-terms/
- Yet another: https://martin-thoma.com/ml-glossary/

# Techniques and Problems

I suppose you may define a problem domain like Machine Learning by describing the problems it solves and the techniques it uses.  
Now both are vast and varied, but let me attempt to list some here, just so you get a sense of what we are into.  

## Common Problems we try to solve

- **Binary Classification**: put an example into one of 2 available classes, for e.g. Object of Type A or B, Student is proficient or not, Yes or Not
- **Multi-class Classification**: put an example into one of many available classes, for e.g. each 'digit' in a set of handwritten numbers can be a class, now we need to predict which of the images belong to which class (and hence represents which number)
- **Prediction or Regression**: Try and predict a value
- **Ranking**: Rank courses, movies, web pages in order of relevance
- ...others
When we break machine learning problems this way, we give ourselves a method for measuring the errors.

## 'Paradigms' or Techniques or 'Types of ML'

You may not care about this *eventually*, but we humans learn by classifying, so here's a common way to bucket the problems of machine learning:

- **Supervised learning**: Input a **vector**, find out what **class**/**lable** the vector belongs to using a **model**. Learn using existing **labelled** data where a variety of vectors have already been assigned labels.
- **Unsupervised learning**: Input a vector, output a **transformed value** (or a vector) that solves a practical problem (for e.g. **clustering, outlier detection, dimensionality reduction** etc.). Learn using data that has no labels.
- **Semi-supervised learning**: Just like supervised learning, input a vector, find out what class/lable the vector belongs to. Learn based on data that has labels, but *a lot of the lables are missing* - you have data that can better inform your probability distributions, so this could improve the classification. 
- **Reinforcement learning**: Pick an action to maximize average/cumulative reward for a given state of the environment. 
- **Ensemble learning**: Improve the performance of your models. Uses tricks from supervised learning.

Here is...

### A visual lay of the land

![A Mindmap of the algorithms](images/MachineLearningAlgorithms.png)
(source: https://machinelearningmastery.com/)


There are several common algorithms that one needs to know. An intution about these is available on [the scikit-learn site](https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html)

![Choosing the right estimator](images/ml_map.png)

Another interesting one is [available from Microsoft](https://download.microsoft.com/download/A/6/1/A613E11E-8F9C-424A-B99D-65344785C288/microsoft-machine-learning-algorithm-cheat-sheet-v7.pdf)

Also:
[A visual introduction to machine learning](http://www.r2d3.us/visual-intro-to-machine-learning-part-1/)


# Topics covered
Here are all the bits we will cover:
- Decision Trees (ready)
- The Confusion Matrix (WIP)
- Regression - Linear Regression (WIP)
- Regression - Logistic Regression (WIP)
- Clustering - K-Means and K-Medians (WIP)
- Dimensionality Reduction - PCA (WIP)
- Dimensionality Reduction - LDA (WIP)
- *more to follow as we develop this further*

# Mechanics
## How the tutorial works
Each bit addressed below will have one or three Jupyter Notebooks associated with them.  
Either:  
- An empty notebook, where you can add your code.
- A tutorial notebook.
- A solution notebook.
You can start with the empty notebook, follow the tutorial and end up with the solution.  
Or you get one notebook, you create a new one in Jupyter and follow the one here.
The notebooks in the repo will be clearly marked and the names would be self explanatory.
## You'll need
- A computer with atleast 16 Gb of RAM
- Access to the internet
- Anaconda installed on your machine: prefer a [64-bit, Python 3.x download from here](https://www.anaconda.com/download/)
- Datasets that we need for each of the exercises are listed [here](dataset-references.md)  


# ML vs AI - a quick rant
I come across this question again and again. IMO, _this is a perfectly useless classification, reserved for sales decks and management retreats. If you really are one of those who want to get to work, ignore this._  

This is how folks around me seem to talk about the two terms:   
- Machine Learning is a 'subset' of AI
	- deals with extant algorithms and their implemetation
	- when people use this term what they mean is not only implementing cool algorithms, but also doing the work of loading and querying data, cleaning it, figuring out the inconsistencies, the idisyncracies of the data/domain, imputing where necessary and the other tasks that may be thought of as 'drudgery' simply because they are the necessary nuts and bolts of every ML operation. This is not unlike the way engineering is treated - where the people writing the code are at the bottom of the pyramid. 
- AI is all the research going on around Intelligent Machines - all the 'Math' work. 
  
Ultimately it's upto the practioner to gain expertise and earn respect. ML vs AI - these divisions are largely there for people, who'll never write code or model with their own hands but need to talk in ways that don't sound completely stupid (to others like them).  