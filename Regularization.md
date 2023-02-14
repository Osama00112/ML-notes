# Regularization

When building a model, we may end up overfitting while trying to minimize the loss of our hypothesis.<br>
One way of avoiding this scenario is to add a measure of complexity to the cost function. <br>
So, _**Regularization**_ is a method of penalizing hypothesis that are more complex to favor simlper, more general hyptheses<br>


> cost(h) = loss(h) + $\lambda *$ complexity(h)

* For simpler decision boundary
* As opposed to something that fits the data better while not generalizing very well
* Need a balance between loss and complexity
* If $\lambda$ is greater, we really want to penalize the "more complex hypothesis"
