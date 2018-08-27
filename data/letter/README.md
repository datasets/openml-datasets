The resources for this dataset can be found at https://www.openml.org/d/6

Author: David J. Slate  
Source: [UCI](https://archive.ics.uci.edu/ml/datasets/Letter+Recognition) - 01-01-1991  
Please cite: P. W. Frey and D. J. Slate. "Letter Recognition Using Holland-style Adaptive Classifiers". Machine Learning 6(2), 1991  

1. TITLE: 
  Letter Image Recognition Data 
 
    The objective is to identify each of a large number of black-and-white
    rectangular pixel displays as one of the 26 capital letters in the English
    alphabet.  The character images were based on 20 different fonts and each
    letter within these 20 fonts was randomly distorted to produce a file of
    20,000 unique stimuli.  Each stimulus was converted into 16 primitive
    numerical attributes (statistical moments and edge counts) which were then
    scaled to fit into a range of integer values from 0 through 15.  We
    typically train on the first 16000 items and then use the resulting model
    to predict the letter category for the remaining 4000.  See the article
    cited above for more details.