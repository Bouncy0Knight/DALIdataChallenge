# DALIdataChallenge

I created a program that uses gower's distance as a metric to cluster the provided dataset. It first imputes the data through K - nearest neighbors twice - once for numerical data, and a second time for categorical data. The imputation steps are tested somewhat extensively through visual analysis. The final clusters allow us to make predictions about the inter-relations of varying dartmouth course factors. Note that this is an unsupervised clustering algorithm.

Following imputation via KNN, the code one-hot encodes the categorical values in the dataset to allow us to implement a clustering algorithm. Before implementing the algorithm, we use the elbow method, which clusters the dataset 9 different times and stores the cost of each clustering attempt. By graphing the cost against the number of clusters, we can predict the optimal number of clusters as the location where the graph hits an inflection point. 

The final function, plot centroids, plots the clustered observations against each other based on varying characteristics passed in. From this it is possible to make novel predictions about the dataset. For example: 

0) the clustering suggests that as the median GPA increases, the chance that a class is an econ class decreases. 
1)As the average section size decreases, the gpa of the class increases. 
2)As the number of sections increases, the average section size increases. 
3)The model predicts that low and high course numbers will have higher GPAs than intermediate course numbers



Successfully running this program locally may require the pip installation (via terminal) of the following packages:
Package           Version
----------------- -------
contourpy         1.0.7
cycler            0.11.0
et-xmlfile        1.1.0
filelock          3.11.0
fonttools         4.39.3
Jinja2            3.1.2
joblib            1.2.0
kiwisolver        1.4.4
kmodes            0.12.2
MarkupSafe        2.1.2
matplotlib        3.7.1
mpmath            1.3.0
networkx          3.1
numpy             1.24.2
openpyxl          3.1.2
packaging         23.1
pandas            2.0.1
Pillow            9.5.0
pip               23.1.2
pyparsing         3.0.9
python-dateutil   2.8.2
pytz              2023.3
scikit-learn      1.2.2
scipy             1.10.1
setuptools        57.4.0
six               1.16.0
sympy             1.11.1
threadpoolctl     3.1.0
torch             2.0.0
typing_extensions 4.5.0
tzdata            2023.3

