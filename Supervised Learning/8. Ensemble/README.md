# Ensemble Methods
The idea behind ensemble methods is fairly simple: why use one model when you can use multiple models?

### Real-World Example
The example given in class made a lot of sense to me, and thus I will use it here. Remember the days when you were a little kid and you were asked to guess how many jellybeans were in a jar. Now, maybe you guessed it right every once in a while, but most of the time you were probably way off the mark, even if you implemented some fancy method where you tried to count the number of jelly beans on the outside of the jar and did the subsequent math given rough volume. However, what is really interesting is that while you as an individual guessed it wrong (and maybe even very wrong), when you average out the guesses of multiple individuals, the answer is very, very close to the real answer.

### Implementation
The same idea applies for machines. As we have seen, sometimes machines spit out extremely questionable results. However, if we randomize the data and ask multiple different machines to classify data using different models, when you average out the results, you get much more accurate answers. 

There are two types of ensemble methods: bagging and random forests, which I will explain in more detail in each of the bagging and random forest modules.

# Bagging
The term Bagging comes from the terms Bootstrap Aggregating.

### Bootstrapping
Bootstrapping is the process of splitting data in random, smaller samples (with replacement) and running various models (like the Decision Tree classifier) on these smaller samples in order to infer results. The image below illustrates the idea of Bootstrapping:
<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fmiro.medium.com%2Fmax%2F2054%2F1*iH5w0MBdiOlxDOCX6nmqqw.png&f=1&nofb=1" height = "80%" width="80%">

### Aggregating
After Bootstrapping occurs, the models are then aggregated to form one comprehensive, more accurate model.

The main idea behind bagging is not that the models themselves are very accurate, but that together they can form a more accurate model. In fact, when implementing bagging, the models we use will be highly simplified and considered "dumb learners" in that their predictions are barely better than random guessing.

<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdataaspirant.com%2Fwp-content%2Fuploads%2F2020%2F09%2F5-Bagging-ensemble-method.png&f=1&nofb=1" height = "80%" width="80%">

### Example
A simple example of bagging is asking amateur wine tasters to taste random samples of wine and rank the best quality wine. While the wine tasters themselves are probably quite inexperienced and might not make very accurate predictions, together their results can be fairly accurate.

# Random Forests
The idea behind Random Forests is very similar to the idea behind Bagging, but with a slight tweak. When implementing bagging, the models use the same set of features to decide where to break off the data. This means that while there may be difference in the results of the models, the models likely split the data at similar places. However, Random Forests adds yet another layer of randomness by having a random set of features instead of the full set of features. This yields more varied results, so that when aggregated, more accurate results are made. It is similar to the idea that if you have a group of people and given some attributes, they all tend to make the wrong assumption, then the data is still skewed. However, if you vary the attributes given, then the data becomes less skewed.

# Task
In this module, I will take many of the same attributes that I have been using in the previous modules (magnesium, non-flavanoid phenols, etc.) to try to classify the different wines in the load wine dataset and see how bagging and random forests performs. I will also try to predict the quality of white wine based on various attributes using bagging and random forests, as well as try to find the most important attributes.
