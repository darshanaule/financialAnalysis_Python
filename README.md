# financialAnalysis_Python
Scatter plot:
I have tried to plot the scatter plot with line of regression(In this case we have non linear regression). To find best plot I tried to plot for different values of degree ranging from 1 to 4 . With this we also get different values of threshold for each degree which can be used to decide the best plot.
The threshold value represents the market capitalization level beyond which quarterly sales tend to increase significantly
Following are brief findings:
- Degree 1 (Linear): Threshold value -8029
    - This suggests that the linear model doesn't capture the relationship well, as the threshold value is negative and doesn't make practical sense. This could be a case of underfitting.
- Degree 2 (Quadratic): Threshold value 1097099
    - This value seems more reasonable, indicating that quarterly sales tend to increase significantly when market capitalization exceeds approximately 1097 billion Crores.
- Degree 3 (Cubic): Threshold value 380669
    - This value is lower than the quadratic model's threshold, which might indicate that the cubic model is capturing a more complex relationship.
- Degree 4 (Quartic): Threshold value 427591
    - This value is close to the cubic model's threshold, suggesting that the quartic model is also capturing a similar complex relationship.

After experimenting and observing the plot with different degrees I choose to go with degree 3 so as to capture maximum complex relationship while avoiding overfitting. 
The cubic model (degree 3) has a threshold value of approximately 380,669. This means that quarterly sales tend to increase significantly when market capitalization exceeds this value.

Cubic models are often more flexible than quadratic models, but less prone to overfitting than higher-degree models like quartic or quintic.
By selecting the cubic model, we are likely to get a better generalization of the data, and the threshold value it provides should be more reliable.

As in  model with  degree 4 polynomial regression line does touch some points on the scatter plot, but doesn't intersect them perfectly. This suggests that the model is capturing the general trend of the data, but might not be fitting each point exactly. This could be a case of overfitting.

- Correlation coefficient (0.61):
    - Indicates a moderate to strong positive linear relationship between market capitalization and quarterly sales.
    - As market capitalization increases, quarterly sales tend to increase as well.
- Coefficient of determination (R^2) (0.37):
    - Suggests that about 37% of the variation in quarterly sales can be explained by the variation in market capitalization.
    - This means that while there is a significant relationship between the two variables, there are still other factors influencing quarterly sales that are not captured by market capitalization alone.


Decision Trees:
Tree plot displays the following parameters for each node:

1. Mar Cap-Crore: This is the feature (or attribute) being used to split the data at this node. In this case, it's the market capitalization in Crores.

2. Squared Error: This is the measure of impurity or variance in the target variable (Quarterly Sales) for the samples in this node. A lower value indicates more homogeneous samples.

3. Samples: This represents the number of data points (samples) that fall within this node.

4. Values: This shows the distribution of the target variable (Quarterly Sales) for the samples in this node. It's usually represented as a list of values, where each value corresponds to a specific class or range of values.


