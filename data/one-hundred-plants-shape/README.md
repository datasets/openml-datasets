The resources for this dataset can be found at https://www.openml.org/d/1492

Author: James Cope, Thibaut Beghin, Paolo Remagnino, Sarah Barman.  
Source: [UCI](https://archive.ics.uci.edu/ml/datasets/One-hundred+plant+species+leaves+data+set) - 2010   
Please cite: Charles Mallah, James Cope, James Orwell. Plant Leaf Classification Using Probabilistic Integration of Shape, Texture and Margin Features. Signal Processing, Pattern Recognition and Applications, in press. 2013.     

### Description

One-hundred plant species leaves dataset (Class = Shape).
 
### Sources
```
   (a) Original owners of colour Leaves Samples:

 James Cope, Thibaut Beghin, Paolo Remagnino, Sarah Barman.  
 The colour images are not included.  
 The Leaves were collected in the Royal Botanic Gardens, Kew, UK.  
 email: james.cope@kingston.ac.uk  
   
   (b) This dataset consists of work carried out by James Cope, Charles Mallah, and James Orwell.  
 Donor of database Charles Mallah: charles.mallah@kingston.ac.uk; James Cope:  james.cope@kingston.ac.uk  
```

### Dataset Information

The original data directory contains the binary images (masks) of the leaf samples (colour images not included).
There are three features for each image: Shape, Margin and Texture.
For each feature, a 64 element vector is given per leaf sample.
These vectors are taken as a contiguous descriptor (for shape) or histograms (for texture and margin).
So, there are three different files, one for each feature problem:  
 * 'data_Sha_64.txt' -> prediction based on shape [dataset provided here]
 * 'data_Tex_64.txt' -> prediction based on texture
 * 'data_Mar_64.txt' -> prediction based on margin  

Each row has a 64-element feature vector followed by the Class label.
There is a total of 1600 samples with 16 samples per leaf class (100 classes), and no missing values.

### Attributes Information

Three 64 element feature vectors per sample.

### Relevant Papers

Charles Mallah, James Cope, James Orwell. 
Plant Leaf Classification Using Probabilistic Integration of Shape, Texture and Margin Features. 
Signal Processing, Pattern Recognition and Applications, in press.

J. Cope, P. Remagnino, S. Barman, and P. Wilkin.
Plant texture classification using gabor co-occurrences.
Advances in Visual Computing,
pages 699-677, 2010.

T. Beghin, J. Cope, P. Remagnino, and S. Barman.
Shape and texture based plant leaf classification. 
In: Advanced Concepts for Intelligent Vision Systems,
pages 345-353. Springer, 2010.
