# Perceptron Model
The first model that we learn in the class was a simple single neuron Perceptron Model. The idea of the perceptron model is much like a simple organism that takes various signals, as well as some personal bias, to output another signal. In fact, the Single Neuron Perceptron Model derives its name from the neurons in our brains that take various signals and output other signals. 
![Perceptron](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fstarship-knowledge.com%2Fwp-content%2Fuploads%2F2020%2F10%2FPerceptrons.jpeg&f=1&nofb=1)

### Here is a simple real-world example of what the Perceptron Model is modelled after: 
Say you are at a fancy party and you have just tried some wine. After tasting the wine, you are trying to determine whether it is a high quality wine or not. There are many factors that you might consider: is the wine sweet? What overtones does it have? Also, there is some personal bias attached to it: do you personally like the taste of the wine? Not all people prefer the same type of wine. After considering these various factors, you would then weight the importance of each attribute: maybe sweetness is a big factor in determining whether or not a wine, for you, is high-quality. Finally, after considering all these different factors, you would make a decision on whether or not this wine is high quality. In fact, the more different types of wine you try, the better you get at deciding whether or not the wine is high-quality or not. This is also very similar to machine learning: the more data the machine can go through, the better it gets at classifying.

The Single Neuron Perceptron Model is used for binary classification. This means that it will input some signals and output one of two answers (this is similar to a "yes" or "no" question). Of course, the Perceptron Model works best for models that have linearly separable data. For data that is not linearly separable, the Single Neuron Perceptron Model has trouble classifying the data. In future models, the models will become more complex and we will explore ways to classify more than two objects, as well as potentially increase efficiency and accuracy. 

![YesNo](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fimage.freepik.com%2Ffree-vector%2Fyes-and-no-signs_1325-370.jpg&f=1&nofb=1)

The model starts by randomly weighting various input signals. Then, it is activated with a preactivation function (we will use a sign activation function in the example), before outputting a post-activation value. Next, we test the accuracy of the data (find error) to better improve our findings and then update the weights of the various input signals. We do this with all our data to get the best classification.

# Task
The task that I will accomplish is very similar to the real-world example I gave for the perceptron model: I will take data from load wine data two classes of wine (Class 1 and 2) and try to determine which class of wine something is based on different attributes.

