# Ensemble Methods
The idea behind ensemble methods is fairly simple: why use one model when you can use multiple models?

### Real-World Example
The example given in class made a lot of sense to me, and thus I will use it here. Remember the days when you were a little kid and you were asked to guess how many jellybeans were in a jar. Now, maybe you guessed it right every once in a while, but most of the time you were probably way off the mark, even if you implemented some fancy method where you tried to count the number of jelly beans on the outside of the jar and did the subsequent math given rough volume. However, what is really interesting is that while you as an individual guessed it wrong (and maybe even very wrong), when you average out the guesses of multiple individuals, the answer is very, very close to the real answer.

### Implementation
The same idea applies for machines. As we have seen, sometimes machines spit out extremely questionable results. However, if we randomize the data and ask multiple different machines to classify data using different models, when you average out the results, you get much more accurate answers. 

There are two types of ensemble methods: bagging and random forests, which I will explain in more detail in each of the bagging and random forest modules.