## Ensemble methods

These ML methods combine multiple weak learners to get a strong learner (or ensemble model). 

Weak learners (or base models) models are models that can be used as building blocks for designing more complex models by combining several of them. Most of the time, these basic models do not perform so well by themselves either because they have a high bias or because they have too much variance to be robust. The idea of ensemble methods is to try reducing bias and/or variance of such weak learners by combining several of them together in order to create a  ensemble model that achieves better performance.

If the same base model is used in all weak learners, the resulting ensemble model is called as homogeneous otherwise it's heterogeneous ensemble.

The main categorization of ensemble methods is

* <b>Bagging</b>: homogeneous weak learners, learnt independently in parallel and combined by deterministic averaging process
* <b>Boosting</b>: homogeneous weak learners, learnt sequentially and in an adaptative way (a base model depends on the previous ones) and combines them using a deterministic strategy
* <b>Stacking</b>: heterogeneous weak learners, learns them in parallel and combines them by training a meta-model to output

Very broadly, bagging aims at an ensemble model with less variance than its components whereas boosting and stacking try to produce strong models less biased than their components (even if variance can also be reduced).

![bagboost](https://github.com/InFoCusp/ml_dl_wiki/src/img/bagboost.png)

### References

1. [Blog on medium](https://towardsdatascience.com/ensemble-methods-bagging-boosting-and-stacking-c9214a10a205)
