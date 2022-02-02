# ML prediction model to classify smokers with and without cancer. 
## Data represents gene expression profiles from epithelial cells from cigarette smokers without cancer, with cancer, and with suspect lung cancer.

We have a dataset of gene expression profile from epithelial cells of ~200 smokers, with or without cancer. The gene expression profile consists of ~22,000 values for each individual (expression value of each gene).
We use this dataset to build a classifier that would predict if a patient has lung cancer, based on his/her gene expression profile.

Here are some points we implemented for an improved classifier and to explore the dataset:
* We ran statistical tests for each gene and saw that there's a significant different expression between patient with and without cancer. This allowed us to choose only relevant features to build the model.
* We clustered and visualized the expression of the ~22k genes, to try and see correlations (group of genes that are expressed together). 
* We want cross-validated our model, and examined how the accuracy parameters changed as a function of how many genes (features) we choose for the model.
* Lastly, we preformed a PCA analysis to try and visually cluster between patients with and without cancer.

### We reached a very satisfying result - our final model has the following parameters:

* True Positive Rate: 0.7083333333333334 
* True Negative Rate: 0.7857142857142857 
* False Positive Rate: 0.21428571428571427 
* False Negative Rate: 0.2916666666666667 
* Accuracy: 0.7368421052631579