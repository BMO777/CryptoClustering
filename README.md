# CryptoClustering
In this repo will be found a Jupyters notebook named Crypto_Clustering.  Pandas-python is used to read a dataframe from csv in the resources directory, then the data is prepared using the standard scaler from scikit python library for preprocessing.

Then using K-means algorithm from the clustering section in the scikit library, an optimal k value is found after creating a list using a fitted model with the scaled data. This is easy to visualize with an elbow curve created using all k values and inertia values converted to a dataframe then plotted with hvplot .

THe best value determined for k(4 in this case) is them initialized using the K-means model, plugging the best value into the n_clusters variable. Then the model is fitted and using .predict, next it is appened to the original dataframe and plotted with hvplot- using the k value to reassign data points according to K-means model predictions.

Next using the statistical technique; Principal Component Analysis, the original data is modeled and fitted. Calculating the explained variance using the fitted PCA info showed 89.5%. The PCA info is also modeled, fitted and predicted using K-eans, then plotted.

Finally, the scaled data and the PCA plots are combined into composite plots for easy comparison of data points.

To run: Python and the libraries scikit, and hvplot are required. Jupyters notebook is the recommended editor and viewer of the notebook file. 

