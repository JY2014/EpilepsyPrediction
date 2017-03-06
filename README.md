# Predicting Epilepsy Diagnosis and Impact Using National Survey of Children's Health
### Harvard University Stat121a Introduction to Data Science Final Project 
### Jingyi Yu, Alexandra Ding, Ziao Lin

Seizures and epilepsy are the most common neurological disorders among children in the United States, and put children at risk of disability, injury, and death. Currently, epilepsy diagnosis relies on patient history and lab examinations, but the lack of clear predictors creates difficulties in targeting treatment to patients at risk. This project attempts to predict epilepsy diagnosis based on the child’s health, demographic, and social characteristics, in order to identify risk factors for epilepsy as well as allow doctors and parents to be more vigilant of early behavioral signs of seizures. In addition to predicting whether children have epilepsy, we also aimed to predict the quality of life of children with epilepsy. 

## This project is presented at https://jy2014.github.io/EpilepsyPrediction/Home.html
<br>
</br>
___
## Please read this if you are trying to run the code:

Before attempting to run code, unzip the data files.

[We could not upload the CSV files without zipping because they are too large. ]
* NSCH_2007.zip
* NSCH_2007_droppedADP_codeLMN.csv.zip
* NSCH_2007_droppedADP_codeLMN_na.csv.zip
* imputed_PovertyLevel_RF.zip


## List of files in this repository:
### Code:
* Website_data_source.ipynb: introduces data source, displays “Data Source” section of website
* website_data_imputation.ipynb : performs missing data imputation; displays “Imputation” section of website
* website_diagnosis.ipynb : Runs classifiers to classify epilepsy status. Displays “Diagnosis” section of website
* website_QOL.ipynb: Runs classifiers to classify Quality of Life within epilepsy patients. Displays “QOL” section of website.

### Datasets:
* NSCH_2007.zip: Raw (zipped) CSV downloaded from NSCH website. (https://www.cdc.gov/nchs/slaits/nsch.htm)
* NSCH_2007_droppedADP_codeLMN.csv.zip: NSCH 2007 with certain columns dropped, some indicators coded (intermediate step during data imputation)
* NSCH_2007_droppedADP_codeLMN_na.csv.zip: NSCH 2007 with certain columns dropped, some indicators coded as NaN values (intermediate step during data imputation)
* Categorical_Column_Names_wState.csv: List of categorical column names, including State. 
* variable_description.csv: CSV containing descriptions of variable names (scraped from PDF; code producing this CSV not included)
* Imputed_PovertyLevel_RF.zip: Dataset with imputed poverty level. This is the dataset we ultimately used in classification. 
* X_select39_epilepsy_for_QOL_non_encode.csv: 39 Selected predictors used in Quality of Life classifier, NOT one hot encoded
* X_select39_epilepsy_for_QOL_onehot.csv: 39 Selected predictors used in Quality of Life classifier, one hot encoded
* y_QOL_binary.csv: binary y values for Quality of life, with values 0 and 1 encoding good and bad.
* y_quality.txt: y values for Quality of Life, with values 0 to 3 encoding good to poor quality of life. 
