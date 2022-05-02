# Gradient Descent
In the Perceptron Model, we explored using a predefined rule to improve our predictions. Gradient descent is a yet another way to optimize our predictions (after all, efficiency is very important in coding!)
![Gradient Descent](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi.stack.imgur.com%2Fw7ARo.png&f=1&nofb=1)

### General Idea of Gradient Descent

To better understand how gradient descent works, I will use a real world example. Because this whole Github repository is centered around wine, I will use the example of wine in a wine glass.

<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.boutiquekozy.ca%2Fwp-content%2Fuploads%2F2018%2F10%2F490407550-U1-Usage-shot.jpg&f=1&nofb=1" width=50% height=50%>

We have probably all seen a while glass: it is shaped like a parabola, with a minimum (or bottom). When we pour wine into the glass, where does the wine go? Does the wine stay on the edges of the wine glass? No, it automatically falls to the bottom of the glass. No matter how we pour the wine, it always ends up at the bottom. Now think of the wine glass like a cost (or error) function. We are trying to minimize the error as much as possible. Thus, we are trying to find the bottom of the wine glass where when we pour the wine, it falls to the bottom.

Now, in actual implementation, we will take the gradient (or first derivative) of a function in order to find a minimum (note: unlike the example of the wine glass which only has one minimum, there can be multiple minimums for a function). Now, we know that to find the minimum, we have to find when the gradient is zero. However, simply finding when the gradient is zero does not guarantee it to be a minimum. It could also be a maximum or saddle point. Thus, to find when a point is a minimum, we also have to test the slopes around it. We know that in order to go towards a minimum, we have to go in the opposite direction of the slope. Of course, now we run into another problem: how far do we go for each step? This is what we call the learning rate (this number we simply have to play around with, which I will do in the implementation of Gradient Descent). Thus, we have found our function:

1. We start by picking a random point in the function (initializing it) and calculating its gradient (or slope). 
2. We go in the opposite direction with a certain sized step (called the learning rate).
3. We calculate the gradient again and keep walking in the opposite direction until we reach the bottom (a threshold around zero).
4. We did it! We found a minimum!

## Limitations of Gradient Descent
As I have said earlier, there can be multiple minimums in a function, but through gradient descent, we are unable to tell whether or not a minimum is a local or global minimum. Thus, gradient descent can get stuck trying to decide between multiple minima.

# Task
In this module, instead of using any large datasets, I will instead just demonstrate the idea behind gradient descent using various functions like the quadratic function and the sine equation. However, I will explain and utilize gradient descent in more detail in the following module for linear regression.
