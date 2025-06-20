# Tea-Classification
Tea aroma classification with feature engineering on time-series data and simple machine learning model.
# Data
The data itself is a time-series data. Where there are 3 types of tea: BOHEA, BOP, and PF with each of them has 3 samples. Each of the sample is put into a machine called electronic nose 5 times. The electronic nose will detect the aroma based on 6 features that has been set in the machine: MQ7, MQ9, TGS822, TGS2600, TGS2602, TGS2611.
![](https://github.com/ThomasArtemius/Tea-Classification/blob/main/Images/BOHEA%20data.png)
![](https://github.com/ThomasArtemius/Tea-Classification/blob/main/Images/BOP%20data.png)
![](https://github.com/ThomasArtemius/Tea-Classification/blob/main/Images/PF%20data.png)
## Data Splitting
The data splitting is relatively straightforward. I use 2 samples from each tea type for training and validation set. The third sample is used for test set.
![](https://github.com/ThomasArtemius/Tea-Classification/blob/main/Images/BOHEA%20data%20splitting.png)
![](https://github.com/ThomasArtemius/Tea-Classification/blob/main/Images/BOP%20data%20splitting.png)
![](https://github.com/ThomasArtemius/Tea-Classification/blob/main/Images/PF%20data%20splitting.png)
From the picture above, I ensure the training data has good variability
# Feature Engineering
Each features in the data are extracted into set of new features that contains information of: mean, standard deviation, median, min, max, range, p25, p75, iqr, skewness, and kurtosis. Because of it, each feature will be extracted become 11 features. Therefore, the total features for the data is 66.
# Methods
Logistic Regression, SVM, and Random Forest
# Result
![](https://github.com/ThomasArtemius/Tea-Classification/blob/main/Images/CM%20Comparison.png)
The data itself is easily classified by nature. Because each features within each tea types has unique range of value.
