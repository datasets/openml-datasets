The resources for this dataset can be found at https://www.openml.org/d/1510

Author: William H. Wolberg, W. Nick Street, Olvi L. Mangasarian    
Source: [UCI](https://archive.ics.uci.edu/ml/datasets/breast+cancer+wisconsin+(original)), [University of Wisconsin](http://pages.cs.wisc.edu/~olvi/uwmp/cancer.html) - 1995  
Please cite: [UCI](https://archive.ics.uci.edu/ml/citation_policy.html)     

Breast Cancer Wisconsin (Diagnostic) Data Set (WDBC). Features are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. They describe characteristics of the cell nuclei present in the image. The target feature records the prognosis (benign (1) or malignant (2)). [Original data available here](ftp://ftp.cs.wisc.edu/math-prog/cpo-dataset/machine-learn/cancer/) 

Current dataset was adapted to ARFF format from the UCI version. Sample code ID's were removed.  

! Note that there is also a related Breast Cancer Wisconsin (Original) Data Set with a different set of features, better known as [breast-w](https://www.openml.org/d/15).


### Feature description  

Ten real-valued features are computed for each of 3 cell nuclei, yielding a total of 30 descriptive features. See the papers below for more details on how they were computed. The 10 features (in order) are:  

a) radius (mean of distances from center to points on the perimeter)  
b) texture (standard deviation of gray-scale values)  
c) perimeter  
d) area  
e) smoothness (local variation in radius lengths)  
f) compactness (perimeter^2 / area - 1.0)  
g) concavity (severity of concave portions of the contour)  
h) concave points (number of concave portions of the contour)  
i) symmetry  
j) fractal dimension ("coastline approximation" - 1)  

### Relevant Papers   

W.N. Street, W.H. Wolberg and O.L. Mangasarian. Nuclear feature extraction for breast tumor diagnosis. IS&T/SPIE 1993 International Symposium on Electronic Imaging: Science and Technology, volume 1905, pages 861-870, San Jose, CA, 1993. 

O.L. Mangasarian, W.N. Street and W.H. Wolberg. Breast cancer diagnosis and prognosis via linear programming. Operations Research, 43(4), pages 570-577, July-August 1995.