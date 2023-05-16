# DALIdataChallenge

I created a program that uses gower's distance as a metric to cluster the provided dataset. It first imputes the data through K - nearest neighbors twice - once for numerical data, and a second time for categorical data. The imputation steps are tested somewhat extensively through visual analysis. The final clusters allow us to make predictions about the inter-relations of varying dartmouth course factors. Note that this is an unsupervised clustering algorithm.

The visual depictions and analyses went incredibly well - the imputations were very strongly supported by the distributions. The program is an unsupervised learning model, so next steps to improve would include training a supervised learning model from the clustering data to create novel predictions. This would make the predictions and analyses much more robust.

I'm most proud of the imputation steps - I'm less experienced in that area, and it was gratifying to see it go so well. Accordingly, much of what I learned over this project is about the techniques and intuition necessary for conducting imputation.



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

