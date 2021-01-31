## Bagging 

Bagging is an ensemble method that combines weak learners with high variance fitted on subsets of the full data by some form of averaging so as to get a resultingh low variance ensemble. The base models are low bias high variance (overfitted) models that are each fitted on bootstrapped subsets of the full data. 

These data subsets are independent of each other (uncorrelated) and identically distributed (mimic the full dataset distribution as much as possible). Such subsets (having representativity and independence) formed by randomly drawing samples with replacement from the full set are referred to as bootstrap samples in statistics. 

![bootstrapping](https://raw.githubusercontent.com/InFoCusp/ml_dl_wiki/main/src/img/bootstrap.png)
Bootstrapping [1]

There are multiple ways to aggregate the base models: 
* For a regression problem, the outputs of individual models can literally be averaged. 
* For classification problem, there are 2 options:
  * The class that receives the majority of the votes is returned by the ensemble model (this is called hard-voting). 
  * We can also average these class probabilities of all models and keep the class with the highest average probability (this is called soft-voting). 
Averages or votes can either be simple or weighted if any relevant weights can be used.

One main advantage of  bagging is that the models are independent and hence can be trained in parallel. 


![Bagging](https://raw.githubusercontent.com/InFoCusp/ml_dl_wiki/main/src/img/bagging.png)
Bagging [1]

### References
1. [Post on medium](https://towardsdatascience.com/ensemble-methods-bagging-boosting-and-stacking-c9214a10a205)
