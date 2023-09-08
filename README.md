
---
# *<center>Textile Product Waste Prediction</center>*

*This project aims to optimize production in a textile factory.*
*For various reasons during production, some products are of a quality that cannot be delivered to the customer.*
*For this reason, more products are produced than the number of orders.*
*In this project, it will be predicted how many more products should be produced than the number of orders.*

---

### *Dataset*
*The dataset used in this project was provided by the customer.*

---

### *Version*

- _Python Version: **3.10.8**_
- _Numpy Version: **1.23.5**_
- _Pandas Version: **1.5.2**_
- _Matplotlib Version: **3.6.2**_
- _Seaborn Version: **0.12.1**_
- _Sklearn Version: **1.2.0**_
- _Tensorflow Version: **2.10.0**_
- _Joblib Version: **1.1.1**_

---

# *<center>Folders</center>*

---

## *PreAnalysis*

### - RawDataPreparation
The first data preparation phase.
At this phase, the data was read from Excel and its features were renamed.
See <ins>_/PreAnalysis/RawDataPreparation_</ins> folder for details.

### - Preparation
The phase where data was prepared for training.
At this phase, features and rows that were unusable were deleted, useful information was extracted from the data and defined as new features.
See <ins>_/PreAnalysis/Preparation</ins> folder for details.

### - DataAnalysis
The phase where data was examined.
At this phase, the data prepared for the training was examined in detail by drawing charts.
In addition, in this phase, it was tried to make sense of the data by trying to make inferences from the data examined.
See <ins>_/PreAnalysis/DataAnalysis</ins> folder for details.

### - Training
The phase where training was performed.
A simple neural regression model was trained just for observation  purposes during the Training phase in the PreAnalysis phase.
See <ins>_/PreAnalysis/Training</ins> folder for details.


## *Product*

### - RawDataPreparation
The first data preparation phase.
At this phase, the data was read from Excel and its features were renamed.
See <ins>_/Product/RawDataPreparation_</ins> folder for details.

### - Preparation
The phase where data was prepared for training.
At this phase, features and rows that were unusable were deleted, useful information was extracted from the data and defined as new features.
See <ins>_/Product/Preparation</ins> folder for details.

### - DataAnalysis
The phase where data was examined.
At this phase, the data prepared for the training was examined in detail by drawing charts.
In addition, in this phase, it was tried to make sense of the data by trying to make inferences from the data examined.
See <ins>_/Product/DataAnalysis</ins> folder for details.

### - AnalysisFAMD
The phase where the Factor Analysis of Mixed Data _**(FAMD)**_ method is applied on the data only for observation purposes.
At this phase, the FAMD method was applied to all data without the Train-Test split process and the correlations were examined with charts.
This phase was carried out for observation purposes only, the data was not used in training as it is.
See <ins>_/Product/AnalysisFAMD</ins> folder for details.

### - DataSplit
The phase where Train-Test split process is performed.
Since the prediction process will be repeated with more than one method, splitting the data at this phase will allow the performance of the methods to be compared.
See <ins>_/Product/DataSplit</ins> folder for details.

### - Training
The phase where training was performed.
At this phase, more than one regression model was trained with the splitted data, validation and testing processes were performed and the results were visualized.
Models are splitted into two group models, that only predict SecondQualityRate _**(SingleOutput)**_ and models that predict all error rates at once _**(MultiOutput)**_.
A Linear Regression, Ridge Regression, Polynomial Regression, SVR and Neural Regression models were trained in both groups and recorded with their results.
Then, Weighted Average Ensemble pipeline was created using the saved models and their results, and new predictions were made on test data.
See <ins>_/Product/Training</ins> folder for details.

---

## <center>_I'd Be Glad If You Report Any Mistakes You Notice._</center>

---