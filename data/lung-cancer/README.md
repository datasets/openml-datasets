The resources for this dataset can be found at https://www.openml.org/d/163

Author:   
Source: Unknown -   
Please cite:   

1. Title: Lung Cancer Data
 
 2. Source Information:
 	- Data was published in : 
 	  Hong, Z.Q. and Yang, J.Y. "Optimal Discriminant Plane for a Small
 	  Number of Samples and Design Method of Classifier on the Plane",
 	  Pattern Recognition, Vol. 24, No. 4, pp. 317-324, 1991.
 	- Donor: Stefan Aeberhard, stefan@coral.cs.jcu.edu.au
 	- Date : May, 1992
 
 3. Past Usage:
 	- Hong, Z.Q. and Yang, J.Y. "Optimal Discriminant Plane for a Small
           Number of Samples and Design Method of Classifier on the Plane",
           Pattern Recognition, Vol. 24, No. 4, pp. 317-324, 1991.
 	- Aeberhard, S., Coomans, D, De Vel, O. "Comparisons of 
 	  Classification Methods in High Dimensional Settings", 
 	  submitted to Technometrics.
 	- Aeberhard, S., Coomans, D, De Vel, O. "The Dangers of 
 	  Bias in High Dimensional Settings", submitted to
 	  pattern Recognition.
 
 4. Relevant Information:
 	- This data was used by Hong and Young to illustrate the 
 	  power of the optimal discriminant plane even in ill-posed
 	  settings. Applying the KNN method in the resulting plane	
 	  gave 77% accuracy. However, these results are strongly
 	  biased (See Aeberhard's second ref. above, or email to
 	  stefan@coral.cs.jcu.edu.au). Results obtained by
 	  Aeberhard et al. are : 
 	  RDA : 62.5%, KNN 53.1%, Opt. Disc. Plane 59.4%
 
 	  The data described 3 types of pathological lung cancers.
 	  The Authors give no information on the individual
 	  variables nor on where the data was originally used.
 
        -  In the original data 4 values for the fifth attribute were -1.
           These values have been changed to ? (unknown). (*)
        -  In the original data 1 value for the 39 attribute was 4.  This
           value has been changed to ? (unknown). (*)
     
 	  
 5. Number of Instances: 32
 
 6. Number of Attributes: 57 (1 class attribute, 56 predictive)
 
 7. Attribute Information:
 
 	attribute 1 is the class label.
 	
 	- All predictive attributes are nominal, taking on integer 
 	  values 0-3
 
 8. Missing Attribute Values: Attributes 5 and 39 (*)
 
 9. Class Distribution:
 	- 3 classes, 
 		1.)	9 observations
 		2.)	13     "
 		3.)	10     "
 

 Information about the dataset
 CLASSTYPE: nominal
 CLASSINDEX: first