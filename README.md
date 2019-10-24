# adult_income_prediction
In this analysis we will be trying to obtain the best possible model to classify based on the income whether greater than 50K or less than 50K.

Firstly we will be analysing the given dataset by finding any discrprncies in any feature columns.

We will study the dataset to find if there are any missing values, if found we have to analyse them to decide whether to replace them or remove them. Remember removing the missing values is not always the option. Sometimes removing the values can drastically affect the training dataset which may ultimately affect the model accuracy. Hence we need to study them closely and then decide how to deal with them.

We need to study the correlation between all the feature values. Sometimes there are repetative feautre columns but with different names. If the correlation between the features is found to be close to 1 then we can safely remove one of them while keeping the other. As removing any one will not affect the performance drastically. This is called FEATURE REDUCTION.

This dataset has categorical values too. The problem with most of the categorical values is repitation of the same class with different name. To ease our analysis we can combine some of the classes into single class.

For simplicity to deal with the categorical values i have used get_dummies method of pandas dataframe. There are other various methods that you can use to deal with categorical values.

FEATURE SELECTION is another important concept which we need to understand while analysing data. So features may not contribute to the output of our model. But if include they can affect the result in a not so good way. Hence we need to remove such features and choose only those that drastically affect the output. Again there are different ways in which FEATURE SELECTION can be done. But here i have used Univariate feature selection and Recurssive feature elimination with cross validation.


