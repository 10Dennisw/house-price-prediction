This GitHub repository highlights how I created a model to predict house price prediction. The repository shows:
- Data Exploration
- Feature Engineering
- Building an Extreme Gradient Boosting (XGBoost) Model
  
<u>XGBoost overview.</u>

- XGBoost is a decision tree algorithm which builds upon weak learners.
- The algorithm builds new models to correct the errors made by previous models, by using gradient boosting.
- The trees are built in a greedy manor, selecting the best split to optimise the objective function.
- XGBoost includes L1 (Lasso Regression) and L2 (Ridge regression) regularisation to prevent overfitting.
- Additionally, XGBoost uses cross-validation to improve the generalisation performance of the result. 

To provide mathematical details, XGBoost minimising the equation below through gradient descent to build a tree:

$$
\left[ \sum_{i=1}^{n} L(y_{i},p_{i})\right] + \gamma T + \frac{1}{2}\lambda\mathrm{O}_{2}^{value}
$$

Equation Breakdown:
- Loss Function: $L(y_{i},p_{i})$
- Tree Pruning: $\gamma T$
- Regularisation Term: $\frac{1}{2}\lambda\mathrm{O}_{2}^{value}$
