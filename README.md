# DecisionTree
Building the Decisoin Tree (classification tree and regression tree) by ASD data. It is just a test demo which can help us to be familiar the process of building this model.

You just need to run the Decision_Tree_ASD.ipynb, and then you can get a classification tree and a regression tree of the ASD data.

Attention please: 
  It is just a sample demo to build the decision tree. There also are many thoughtless places like:
  1. I am not sure if you noticed that we are using 'pandas.Categorical(XX.columns).codes' to handle the non-numeric attribute. Indeed, it can easily help us achieve our goals, but if we want to validate our model with a validation set, how can we use the same standard to convert attributes to corresponding numbers. It's possible to use '.codes' again, but once the attribute has a new value (we don't know), the result will completely deviate from our expectations. Then it seems necessary to establish a mapping cross reference table.
  2. Lack of validation set, our model will probably over fit. How to prune to help us improve the robustness of the model?
