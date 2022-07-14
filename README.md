# Breast Cancer Binary Classification using Pytorch

According to the American Cancer Society, each year on average about 200k people discovers that they have invasive breast cancer. Out of all the breast cancer cases detected yearly, about 80% are due to invasive ductal carcinoma (IDC), also known as infiltrating ductal carcinoma. IDC, is a cancer that will begin growing in the milk duct (“pipes” that that carry milk from the milk-producing lobules to the nipple) and later spread to the surrounding fatty tissue of the breast outside the duct. IDC is more prevalent among women as they grow older. In some cases, IDC can also affect men.

Data Source
We have used publicly available dataset Breast Cancer Wisconsin and have download from UCI Machine Learning Repository. Repository: https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29.
The data, in csv format, can be downloaded from this link


Here, we are just giving you description about it.

There are 569 rows in total, each with 31 columns.
The first column is an ID that identifies each patient.
Diagnosis is a categorical variable.
Missing attribute values: none
The second column is the diagnosis of the tumor and it has two possible values: B means that the tumor was found to be benign. M means that it was found to be malignant.
Out of the 569 patients in the dataset, the class distribution is: Benign: 357 (63%) and Malignant: 212 (37%)
This is useful information that allows us to achieve some conclusions.

Our objective will be to train our models to predict if a tumor is benign or malignant, based on the features we derive from dimensionality reduction.
We will not make use of the first column that holds the ID of the patient.
In binary classification scenarios, It’s good to have a good percentage of data from both classes. We have a 70%-30% distribution, which is good enough.
The benign and malignant classes are identified with the characters B and M. We will change the values of the class columns to hold a 0 instead of a B for benign cases and a 1 instead of a M for malignant cases.
