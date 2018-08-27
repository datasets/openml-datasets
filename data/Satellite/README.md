The resources for this dataset can be found at https://www.openml.org/d/40900

Author: Markus Goldstein  
Source: [Dataverse](http://www.madm.eu/downloads https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/OPQMVF)  
Please cite:   

The satellite dataset comprises of features extracted from satellite observations. In particular, each image was taken under four different light wavelength, two in visible light (green and red) and two infrared images. The task of the original dataset is to classify the image into the soil category of the observed region. 

### Classes
We defined the soil classes “red soil”, “gray soil”, “damp gray soil” and “very damp gray soil” as the normal class. From the semantically different classes “cotton crop” and “soil with vegetation stubble” anomalies are sampled. 

After merging the original training and test set into a single dataset, the resulting dataset contains 5,025 normal instances as well as 75 randomly sampled anomalies (1.49%) with 36 dimensions 

### Relevant Papers

Goldstein, Markus, and Seiichi Uchida. A comparative evaluation of unsupervised anomaly detection algorithms for multivariate data." PloS one 11.4 (2016): e0152173 

This dataset is not the original dataset. The target variable 'Target' is relabeled into 'Normal' and 'Anomaly'