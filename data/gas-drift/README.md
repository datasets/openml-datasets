The resources for this dataset can be found at https://www.openml.org/d/1476

Author: Alexander Vergara  
Source: [UCI](https://archive.ics.uci.edu/ml/datasets/gas+sensor+array+drift+dataset) - 2012    
Please cite: Alexander Vergara, Shankar Vembu, Tuba Ayhan, Margaret A. Ryan, Margie L. Homer, Ramón Huerta. Chemical gas sensor drift compensation using classifier ensembles, Sensors and Actuators B: Chemical (2012) doi: 10.1016/j.snb.2012.01.074.   

### Description
Gas Sensor Array Drift Dataset Data Set

### Sources
```
(a) Creators: Alexander Vergara (vergara '@' ucsd.edu) 
BioCircutis Institute 
University of California San Diego 
San Diego, California, USA 

(b) Donors: Alexander Vergara (vergara '@' ucsd.edu) 
Ramon Huerta (rhuerta '@' ucsd.edu) 
```

### Dataset Information

This archive contains 13910 measurements from 16 chemical sensors utilized in simulations for drift compensation in a discrimination task of 6 gases at various levels of concentrations.  
The goal is to achieve good performance (or as low degradation as possible) over time, as reported in the paper mentioned below in Section 2: Data collection. 

The primary purpose of providing this dataset is to make it freely accessible online to the chemo-sensor research community and artificial intelligence to develop strategies to cope with sensor/concept drift. The dataset can be used exclusively for research purposes. Commercial purposes are fully excluded.

The dataset was gathered within January 2007 to February 2011 (36 months) in a gas delivery platform facility situated at the ChemoSignals Laboratory in the BioCircuits Institute, University of California San Diego. 

Being completely operated by a fully computerized environment controlled by a LabVIEW's National Instruments software on a PC fitted with the appropriate serial data acquisition boards. The measurement system platform provides versatility for obtaining the desired concentrations of the chemical substances of interest with high accuracy and in a highly reproducible manner, minimizing thereby the common mistakes caused by human intervention and making it possible to exclusively concentrate on the chemical sensors for compensating real drift.

The resulting dataset comprises recordings from six distinct pure gaseous substances, namely Ammonia, Acetaldehyde, Acetone, Ethylene, Ethanol, and Toluene, each dosed at a wide variety of concentration values ranging from 5 to 1000 ppmv. An extension of this dataset with the concentration values is available at [Gas Sensor Array Drift Dataset at Different Concentrations Data Set](http://archive.ics.uci.edu/ml/datasets/Gas+Sensor+Array+Drift+Dataset+at+Different+Concentrations).


### Attribute Information

The response of the said sensors is read-out in the form of the resistance across the active layer of each sensor. Hence each measurement produced a 16-channel time series, each of which represented by an aggregate of features reflecting all the dynamic processes occurring at the sensor surface in reaction to the chemical substance being evaluated. 

In particular, two distinct types of features were considered in the creation of this dataset: 
(i) The so-called steady-state feature (Î”R), defined as the difference of the maximal resistance change and the baseline and its normalized version expressed by the ratio of the maximal resistance and the baseline values when the chemical vapor is present in the test chamber; and 
(ii) an aggregate of features reflecting the sensor dynamics of the increasing/decaying transient portion of the sensor response during the entire measurement procedure under controlled conditions, namely the exponential moving average (emaÎ±). These aggregate of features is a transform, borrowed from the field of econometrics originally introduced to the chemo-sensing community by Muezzinoglu et al. (2009), that converts the said transient portion into a real scalar, by estimating the maximum value â€”minimum for the decaying portion of the sensor responseâ€” of its exponential moving average (emaÎ±), with an initial condition set to zero and a scalar smoothing parameter of the operator, Î±, that defines both the quality of the feature and the time of its occurrence along the time series the scalar, set to range between 0 and 1. In particular, three different values for Î± were set to obtain three different feature values from the pre-recorded rising portion of the sensor response and three additional features with the same Î± values but for the decaying portion of the sensor response, covering thus the entire sensor response dynamics. 

For a more detailed analysis and discussion on these features as well as a graphical illustration of them please refer to Section 2.3 and Figure 2, respectively of the annotated manuscript.

Once the abovementioned features are calculated, one is to form a feature vector containing the 8 features extracted from each particular sensor multiplied by the 16 sensors considered here. In the end, there is a resulting 128-dimensional feature vector containing all the features indicated above.

There are six possible classes: 
```
1: Ethanol 
2: Ethylene  
3: Ammonia 
4: Acetaldehyde 
5: Acetone 
6: Toluene
```
### Relevant Papers

Alexander Vergara, Shankar Vembu, Tuba Ayhan, Margaret A. Ryan, Margie L. Homer and Ramón Huerta, Chemical gas sensor drift compensation using classifier ensembles, Sensors and Actuators B: Chemical (2012) doi: 10.1016/j.snb.2012.01.074. 
