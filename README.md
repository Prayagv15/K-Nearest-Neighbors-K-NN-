# K-Nearest-Neighbors (K-NN)
I have applied the K-Nearest Neighbours algorithm. K-NN is a supervised multi-class classifier model. While building the K-NN model we have to be careful in data cleaning, outlier treatment and data should be normalized.

**Objective:** 
- Let's say that new animals are going to be added to the zoo, but we want to know to **_Class_** they belong. As a result, we employ the K-NN algorithm for this identification since it relies on similarity metrics. The K-NN model will look for the traits in the new datasets that are comparable to those of the animals currently in the zoo, and based on those features, it will classify the animals into the appropriate group.

**Outline of the dataset.**

* The dataset consists of 101 animals from the zoo.
* There are various characteristics to describe the animal. All the characteristics, except legs are classified as binary values (1-Present/0-Absent). Except for legs which is given as a count of legs for a particular animal.
* There are 7 different **_Classes_**.

**Instruments for evaluating the model's accuracy**

* In order to tune the hyperparameters, I used *GridSearchCV*, and I chose the best estimator with the highest possible score. The metric, is Euclidean distance according to Minkowski's inequality with p=2.
* I have plotted the plots for accuracy results and error rates.

**The observations are as follows:**

* The model accuracy is very good for the lower values of K and as the value increases the accuracy goes on *decreasing*. Also, the error rate *increases* with higher values of K. After hyperparameter tuning, the optimal value of *K* is 3.
* The *accuracy* of the model was determined to be *94%* during the performance evaluation.
* From the classification report, we observe *precision* and *recall* scores for each **Class**.
* The *confusion matrix* makes it crystal clear why the accuracy isn't 100% because some of the animals are markered into a different *Class*.
