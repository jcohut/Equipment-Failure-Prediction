# What exactly was the process followed?

### Step 1 - Load the data and look inside. 
You'll be surprised at all the details presented to you. I spent a good amount of time trying to understand what the data had to say.
### Step 2 - Data processing
Remove anything that you feel may corrupt your model. There were a ton of NaN values in the given data set. I replaced all of them with 0s.
In some situations, you may want to remove them. Sometimes, it may be useful to impute values in place of the NaNs.
By now, you should have a fair idea of what you are working with. The rest of the game should move like clockwork.
### Step 3 - Extract the features.
You are building a predictive model. You need features. 
Where to look for them? The data themseleves are the features. Each column holds a significance you may not know when you design the model.
Towards the end, I have shown the important features using Explainable AI.

### Step 4 - The Learning algorithm
Choosing the algorithm depends on a number of factors. If you have a lot of data, you can go for a neural network model. 
If you have a tabular data, you can go for tree based approaches. Since the given dataset was imbalanced, I even experimented with a 1-class
SVM. I have shown the model with the best prediction scores in the IPython notebook.

### Step 5 - Interpreting the results
I used SHAP - an explainabel AI tool to identify the most important features. Doing so, I can understand why my model made a certain prediction.
