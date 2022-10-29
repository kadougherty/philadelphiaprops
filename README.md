# philadelphiaprops

The goal of this project is to predict the value of single family homes for the average home buyer/owner in Philadelphia and to identify features that drive up home value.

Property data was sourced from OpenDataPhilly and the City of Philadelphia Office of Property Assement: https://www.phila.gov/property/data/#

Information on features in the dataset were downloaded from this url: https://metadata.phila.gov/#home/datasetdetails/5543865f20583086178c4ee5/representationdetails/55d624fdad35c7e854cb21a4/

In addition to the above dataset, additional information on school locations was used to calculate proximity to schools: https://www.opendataphilly.org/dataset/schools/resource/8e1bb3e6-7fb5-4018-95f8-63b3fc420557

A geojson file to produce a map of Philadelphia county was downloaded from OpenDataPhilly: https://www.opendataphilly.org/dataset/zip-codes/resource/825cc9f5-92c2-4b7c-8b4e-6affa41396ee

Repo organization:

The approach and conclusions are detailed in report_philadelphiaprops.pdf.
Data files are included in interim_data/, and model object files are in models/. Images included in the report and slidedeck are located in plots/

All analysis was written and saved to Jupyter notebooks using Jupyter lab. These were generated as follows:

1. wrangle.ipynb : loaded raw data set, filtered to include only single family homes, cleaned data (see Approach in report)

2. eda.ipynb: explored the distributions of features in the dataset, and their relationship with the target variable (market value)

3. model_development.ipynb: trained a linear regression model and 4 tree-based regression models. evaluated performance of the models

4. evaluate.ipynb: looked at which features were most important to predict market value for final model; investigated where model fails

![map 001](https://user-images.githubusercontent.com/7513318/198849826-b642a9a3-660f-47bd-8054-8842c2d4e1e2.png)


