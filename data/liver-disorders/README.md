The resources for this dataset can be found at https://www.openml.org/d/8

Author: BUPA Medical Research Ltd. Donor: Richard S. Forsyth   
Source: [UCI](https://archive.ics.uci.edu/ml/datasets/Liver+Disorders) - 5/15/1990  
Please cite: 

BUPA liver disorders
 
The first 5 variables are all blood tests which are thought to be sensitive to liver disorders that might arise from excessive alcohol consumption.  Each line in the dataset constitutes the record of a single male individual. 

Important note: The 7th field (selector) has been widely misinterpreted in the past as a dependent variable representing presence or absence of a liver disorder. This is incorrect [1]. The 7th field was created by BUPA researchers as a train/test selector. It is not suitable as a dependent variable for classification. The dataset does not contain any variable representing presence or absence of a liver disorder. Researchers who wish to use this dataset as a classification benchmark should follow the method used in experiments by the donor (Forsyth & Rada, 1986, Machine learning: applications in expert systems and information retrieval) and others (e.g. Turney, 1995, Cost-sensitive classification: Empirical evaluation of a hybrid genetic decision tree induction algorithm), who used the 6th field (drinks), after dichotomising, as a dependent variable for classification. Because of widespread misinterpretation in the past, researchers should take care to state their method clearly.
 
Attribute information  
    1. mcv mean corpuscular volume  
    2. alkphos alkaline phosphotase  
    3. sgpt alanine aminotransferase  
    4. sgot  aspartate aminotransferase  
    5. gammagt gamma-glutamyl transpeptidase  
    6. drinks number of half-pint equivalents of alcoholic beverages drunk per day  
    7. selector field created by the BUPA researchers to split the data into train/test sets  

[1] McDermott & Forsyth 2016, Diagnosing a disorder in a classification benchmark, Pattern Recognition Letters, Volume 73. Note Forsyth is named on the UCI page as the original donor of the dataset.