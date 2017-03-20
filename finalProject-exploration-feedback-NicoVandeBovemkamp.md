### ***Final Project - Exploratory Analysis Feedback***

***Nico Van de Bovenkamp***
***

**Overall:** This notebook is a great start to working with your dataset, cleaning some stuff up, and gaining some insight! And you made great use of python functionality and those For loops! Fantastic use of binning and extracting those titles too!

**Analysis going forward:** Next up, you will build your classifier(s!) on survived! Models learn exceptionally differently, so I would try for something linear (a Logistic Regression with Statsmodels API for some more statistical insight and/or a linear SVM), then move on to non-linear models (Random Forrest, Gradient Boosted Trees, etc.).

**Some Notes and Thoughts:**

* **Feature Importance:** One nice feature of random forests, is the ability to use, and then plot, the `.feature_importance_` of each feature (usually calculated via lowest entropy or gini coeffient). In These types of *why and what factors influence [blank]* problems, the prediction power of a feature can be very handy!
* **Imputing Means** Amazing work with imputing those means. That is a very, very creative way to impute the mean without disturbing the distribution of your data, in fact you even make it a bit more normal. Very nice. Personally, I have never done that, but I may make use of that technique going forward! Again, always be mind
that you should try and apply a difference of means test to validate if the mean is, or is not, significantly different.
* **Model Tuning:** Always remember your Train/Test Split, Regularization, Cross-Validation, Visualizing learning paths, etc.

***A Table of Key Evaluation Metrics and Visuals:***

*Throwing this in here too! Below is a brief set of many ways you can communicate/measure results that will be useful for your final project. Please let me know if you have any questions!*

| Metrics | |
|--- | --- |
| *Classification* | Accuracy, Precision, Recall, AUC Score, Lift, F-Score, Log-Loss, Gini, Entropy/Information Gain, Statistical Significance (p-value) |
| *Regression* | Mean Squared Error, Mean Absolute Error, Log-Likelihood Estimation, Statistical Significance (p-value) |

| Visualizations | |
|--- | --- |
| *Model Tuning* | Learning Curves, Regularization Learning Paths with an Error Metric, Model Error stepwise increasing feature set size |
| *Classification* | ROC Curve, Feature Importance Charts, Lift Curves, Expected Value Plots |
| *Regression* | Residual plots(!), KDE and KDE of Predicted Values, Expected Value |
