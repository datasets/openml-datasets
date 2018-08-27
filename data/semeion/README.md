The resources for this dataset can be found at https://www.openml.org/d/1501

Author: Semeion Research Center of Sciences of Communication     
Source: [UCI](http://archive.ics.uci.edu/ml/datasets/semeion+handwritten+digit)     
Please cite: Semeion Research Center of Sciences of Communication, via Sersale 117, 00128 Rome, Italy 
Tattile Via Gaetano Donizetti, 1-3-5,25030 Mairano (Brescia), Italy.    

### Dataset Description

Semeion Handwritten Digit Data Set, where 1593 handwritten digits from around 80 persons were scanned and documented. The each of the 256 variables V1 - V256 describe one of the pixels and their corresponding values. 

### Sources

The dataset was created by Tactile Srl, Brescia, Italy (http://www.tattile.it) and donated in 1994 to Semeion Research Center of Sciences of Communication, Rome, Italy (http://www.semeion.it), for machine learning research. 

For any questions, e-mail Massimo Buscema (m.buscema '@' semeion.it) or Stefano Terzi (s.terzi '@' semeion.it)

### DataSet Information

A total of 1593 handwritten digits from around 80 persons were scanned, stretched in a rectangular box 16x16 in a gray scale of 256 values. Then each pixel of each image was scaled into a boolean (1/0) value using a fixed threshold. 

Each person wrote in a paper all the digits from 0 to 9, twice. The commitment was to write the digit the first time in the normal way (trying to write each digit accurately) and the second time in a fast way (with no accuracy). 

The best validation protocol for this dataset seems to be a 5x2CV, 50% Tune (Train +Test) and completely blind 50% Validation

### Attribute Information

This dataset consists of 1593 records (rows) and 256 attributes (columns). 
Each record represents a handwritten digit, originally scanned with a resolution of 256 grays scale (28). 
Each pixel of the each original scanned image was first stretched, and after scaled between 0 and 1 (setting to 0 every pixel whose value was under the value 127 of the grey scale (127 included) and setting to 1 each pixel whose original value in the grey scale was over 127). 
Finally, each binary image was scaled again into a 16x16 square box (the final 256 binary attributes).

### Relevant Papers

M Buscema, MetaNet: The Theory of Independent Judges, in Substance Use & Misuse 33(2)1998, pp 439-461.