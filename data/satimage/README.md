The resources for this dataset can be found at https://www.openml.org/d/182

Author: Ashwin Srinivasan, Department of Statistics and Data Modeling, University of Strathclyde  
Source: [UCI](https://archive.ics.uci.edu/ml/datasets/Statlog+(Landsat+Satellite)) - 1993  
Please cite: [UCI](https://archive.ics.uci.edu/ml/citation_policy.html)  

The database consists of the multi-spectral values of pixels in 3x3 neighbourhoods in a satellite image, and the classification associated with the central pixel in each neighbourhood. The aim is to predict this classification, given the multi-spectral values. In the sample database, the class of a pixel is coded as a number. 

One frame of Landsat MSS imagery consists of four digital images of the same scene in different spectral bands. Two of these are in the visible region (corresponding approximately to green and red regions of the visible spectrum) and two are in the (near) infra-red. Each pixel is a 8-bit binary word, with 0 corresponding to black and 255 to white. The spatial resolution of a pixel is about 80m x 80m. Each image contains 2340 x 3380 such pixels. 

The database is a (tiny) sub-area of a scene, consisting of 82 x 100 pixels. Each line of data corresponds to a 3x3 square neighbourhood of pixels completely contained within the 82x100 sub-area. Each line contains the pixel values in the four spectral bands (converted to ASCII) of each of the 9 pixels in the 3x3 neighbourhood and a number indicating the classification label of the central pixel. 

Each pixel is categorized as one of the following classes:  
1 red soil  
2 cotton crop  
3 grey soil  
4 damp grey soil  
5 soil with vegetation stubble  
6 mixture class (all types present)  
7 very damp grey soil  

NB. There are no examples with class 6 in this dataset.  

The data is given in random order and certain lines of data have been removed so you cannot reconstruct the original image from this dataset.  

### Attribute information  
There are 36 predictive attributes (= 4 spectral bands x 9 pixels in neighborhood).
In each line of data the four spectral values for the top-left pixel are given first followed by the four spectral values for the top-middle pixel and then those for the top-right pixel, and so on with the pixels read out in sequence left-to-right and top-to-bottom. Thus, the four spectral values for the central pixel are given by attributes 17,18,19 and 20. If you like you can use only these four attributes, while ignoring the others. This avoids the problem which arises when a 3x3 neighbourhood straddles a boundary. 

In this version, the pixel values 0..255 are normalized around 0.

Note: it is unclear why the attributes are named Aattr - Fattr in this version, since there are only 4 bands and 9 pixels, naming them A1, B1, C1, D1, A2, B2, C2, D2, ... would have made more sense.  

