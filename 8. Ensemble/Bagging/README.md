# Bagging
The term Bagging comes from the terms Bootstrap Aggregating.

### Bootstrapping
Bootstrapping is the process of splitting data in random, smaller samples (with replacement) and running various models (like the Decision Tree classifier) on these smaller samples in order to infer results. The image below illustrates the idea of Bootstrapping:
[Insert image of bootstrapping here]

### Aggregating
After Bootstrapping occurs, the models are then aggregated to form one comprehensive, more accurate model.

The main idea behind bagging is not that the models themselves are very accurate, but that together they can form a more accurate model. In fact, when implementing bagging, the models we use will be highly simplified and considered "dumb learners" in that their predictions are barely better than random guessing.

[insert image of bagging?]

### Example
A simple example of bagging is asking amateur wine tasters to taste random samples of wine and rank the best quality wine. While the wine tasters themselves are probably quite inexperienced and might not make very accurate predictions, together their results can be fairly accurate.
