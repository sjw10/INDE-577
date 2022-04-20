# K-Nearest Neighbors (KNN)
K-Nearest Neighbors is another model commonly used for classification and regression.

### Parametric vs. Nonparametric
All of the methods that we have used in the past are examples of parametric models. Parametric models often rely on underlying-assumptions within the data and set statistical models. One example of an assumption is the set coefficients used in linear regression. In linear regression, there is the assumption that the data is at least somewhat linear. We have seen that when the data isn't especially linear, we can get some weird results.

However, nonparametric models don't really on assumptions and instead focus on the general tendencies of the data. Although nonparametric models can be slow to run, they are also sometimes better at accurately predicting outputs because they don't have underlying assumptions. K-Nearest Neighbors is an example of a nonparametric model.

### "Birds of a Feather Flock Together"
Understanding this common saying is crucial to understanding how KKN works. The concept is quite simple: similar objects tend to be grouped close together. If we go back to wine, think about the different types of wine (red wine, white wine, etc.), as well as subcategories (Sauvignon, Rose, etc.). How exactly do we as consumers differentiate between the different categories? Do we measure the different acidities and perform regression? No, we probably just compare generally how close the features of an unknown wine are to other known wines and classify that unknown wine in that group. As humans, we are very good at putting things into similar categories without any fancy statistical methods. KNN operates off of a similar idea. It calculates the distances between various points and clusters the points that are closest together as a class. Then, if we want to classify say an unknown wine, we might plot some of its attributes and find the points nearest to it to determine what kind of wine we predict it to be. Of course, determining 

### Real World Applications



### Tasks
Discuss error finding and scikit-learn at some point
