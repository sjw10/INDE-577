# INDE-577 Data Science and Machine Learning
Welcome to the INDE-577 Github Repository of Sarah Wang, a current freshman at Rice University. This Github Repository derives itself from the various lessons learned in Randy Davila's INDE-577 Data Science and Machine Learning Class. 

![machine learning](https://github.com/sjw10/INDE-577/blob/main/machine_learning.jpg)

## Datasets
Most of my code will come from three different datasets. 

The first data set comes from Scikit-Learn's load wine dataset. This dataset categorizes three different classes of wine using various different attributes such as magnesium levels and color intensity. I will use to mainly to perform classification for these classes of wine

The other two main datasets I will be using come from this site here: https://archive.ics.uci.edu/ml/datasets/Wine+Quality

There are two similar datasets contained in this link. One is a comparison of the different kinds of red wine while the other is a comparison of the quality of different kinds of white wine. In this Github repository, I will analyze the components that make up a good wine.

In general, almost all of this repository is centered on wine analysis, and is an in-depth study of various attributes of wine, as well as which features are most important in making a high-quality wine. 
![wine](https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fwww.walkingmountains.org%2Fwp-content%2Fuploads%2F2015%2F09%2FRed-Wine-on-Summer-Day.jpg&f=1&nofb=1)

## Error Analysis
I would like to start by discussing two types of error analysis that I commonly use: the Confusion Matrix and the Classification Report.

### Confusion Matrix
The confusion matrix is a table that analyzes how well the machine/learner performed on classification. Instead of simply giving a percentage of classifications that are classified correctly or incorrectly, the classification matrix breaks the classifications down even further to show how each of the classes is categorized. Below is an image of a classic confusion matrix:
![confusion matrix](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.researchgate.net%2Fprofile%2FSteven_Mcelwee2%2Fpublication%2F327190637%2Ffigure%2Fdownload%2Ffig1%2FAS%3A662947315597312%401535070365706%2FConfusion-matrix-for-binary-classification.png&f=1&nofb=1)

This matrix is extremely relevant to our current situation with COVID-19. As we can see, this matrix breaks down each category into four different components so that we can see exactly how many true positives, false positives, true negatives, and false negatives there are. This way, if there is a high error, we can see where the error originates from. I will be using the confusion matrix from Scikit-Learn.

### Classification Report
Based on our confusion matrix, we can also print out a classification report. Our classification report contains three categories: Precision, Recall, and F1-Score.
**Precision** ($P$) is defined as the number of true positives ($T_p$) over the number of true positives plus the number of false positives ($F_p$):
$$
P = \frac{T_p}{T_p + F_p}
$$

**Recall** ($R$) is defined as the number of true positives ($T_P$) over the number of true positives plus the number of false negatives ($F_n$):
$$
R = \frac{T_p}{T_p + F_n}
$$

There quantities are related to the **$F_1$-score**, which is defined as the harmonic mean of precision and recall:
$$
F_1 = 2 \frac{P\times R}{P+R}
$$


### Tasks
Add load_wine dataset to description
Talk about skicit-learn as well as error measurements
