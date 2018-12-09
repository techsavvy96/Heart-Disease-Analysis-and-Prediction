# Heart-Disease-Analysis-and-Prediction


upyter notebooks and files used to generate the results and plots for the project :-

convert_ssv_to_csv.py: Converts a file with space-separated values into a file with comma-separated values.

join_files.py: Joins files downloaded from the UC Irvine Machine Learning Repository into a single file for processing by the iPython notebook below.

Heart_Disease_Analysis_Complete.ipynb: Jupyter notebook to read in the data, store it in a Pandas dataframe for initial processing and plots, and analyze with a logistic regression model.

The initial processing steps of this project are as follows:

curl -o data/cleveland14.csv https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data

curl -o data/hungarian14r.ssv https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/reprocessed.hungarian.data

curl -o data/switzerland14.csv https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.switzerland.data

curl -o data/long_beach_va14.csv https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.va.data

python convert_ssv_to_csv.py hungarian14r

python join_files.py

The output of join_files.py is file data/heart_disease_all14.csv and is ready for processing by Heart_Disease_Analysis_Complete.ipynb.
