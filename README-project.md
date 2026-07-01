## IRIS CLASSIFIER MODEL
Architecture:- 4 -> 10 -> 3
Learning Rate = 0.01
Backpropagation Method:- Mini-Batch Stochastic Gradient Descent 
Model type = Classifier
Loss Function = Categorical Cross Entropy

Data is loaded using **file path**. 
Model uses train test split function from sckit-learn to automatically shuffle the dataset before assigning. 

Model accuracy is not consistent due to the small size of the dataset. Model test accuracy varies with each data load and
run process. This is mainly oweing to overlap between the iris-virginica and iris-versicolor when it comes to their properties, besides
presence of few outliers in the data. This can be confirmed by noting the maximum errors the model makes are between iris-virginca 
and iris-versicolor and the certainty in the wrong answer is also not near 100%. This means that the model is confused by a data 
point that lies somewhere on that overlap. 

Model accuracy is noted to not fall below 90% and it always gives a >90% accuracy (80/20 train-test split). Average seems to be around 
94% over several runs. Again this is due to to the small size of the dataset. If the model gets one wrong out of 29, accuracy falls to 
96.67%, 93.33% if two are wrong and so on.

