# Decision Trees
Decision Trees are another example of non-parametric models used for classification and regression.
<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fd1jnx9ba8s6j9r.cloudfront.net%2Fblog%2Fwp-content%2Fuploads%2F2015%2F01%2FDecision-Tree-Example-7-Decision-tree-Edureka.png&f=1&nofb=1" height = "80%" width = "80%">

### Real World Example
The idea behind the decision tree is relatively intuitive. We probably have all seen the questionaires that ask us a series of yes or no questions to determine the best possible choice for us. A simple example is like those worksheets you probably filled out in elementary school in order to determine the right animal. The questions might go something like this:

Say your animal is a cat.

- Does your animal breathe air?
- No (if yes, it is a type of fish)
- Can it fly?
- No (if yes, start asking about birds)
- Does it have fur?
- Yes.
- Is it commonly kept as a pet?
- Yes.
- Is it usually kept in a cage?

... and so on until you reach the conclusion that it is a cat. 

In fact, this is similar to the game 20 questions where you try to guess an object in under a series of 20 questions. As we can see, the questions get narrower and narrower with each subsequent question. The same idea works for decision trees in machine learning. The machine splits the data into two categories and keeps splitting until all the data is split into its correct classification.

### Implementation
The implementation for decision trees is fairly intuitive. First, you have to understand how the structure of decision trees work. There are two kinds of elements in a decision tree: nodes and branches. You start at the very top with the root node: all your training data. Next, the machine splits the node into two branches and two new nodes. These nodes also fall into two categories: decision nodes and leaf nodes. Decision nodes can be split further into the correct category while leaf nodes are fully classified. Each branch-off is one depth. The computer then continues to sort the nodes until it classifies all the data or until a max-depth is satisfied.

### Potential issues
Decision trees are an extremely easy way to classify data and classify data relatively accurately. However, the problem with decision trees is that because they can continuously sort data until a decision is made, they are notorious for overfitting data. Decision trees tend to place too much emphasis on outliers.

# Task
In this module, I will take many of the same attributes that I have been using in the previous modules (magnesium, non-flavanoid phenols, etc.) to try to classify the different wines in the load wine dataset and see how the Decision Tree performs.
