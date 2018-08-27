The resources for this dataset can be found at https://www.openml.org/d/1500

Author: Sikora M., Wrobel L.     
Source: UCI   
Please cite:  Sikora M., Wrobel L.: Application of rule induction algorithms for analysis of data collected by seismic hazard monitoring systems in coal mines. Archives of Mining Sciences, 55(1), 2010, 91-114.  

* Title: 

seismic-bumps Data Set 

* Abstract: 

The data describe the problem of high energy (higher than 10^4 J) seismic bumps forecasting in a coal mine. Data come from two of longwalls located in a Polish coal mine.

* Source:

Marek Sikora^{1,2} (marek.sikora '@' polsl.pl), Lukasz Wrobel^{1} (lukasz.wrobel '@' polsl.pl) 
(1) Institute of Computer Science, Silesian University of Technology, 44-100 Gliwice, Poland 
(2) Institute of Innovative Technologies EMAG, 40-189 Katowice, Poland


* Data Set Information:

Mining activity was and is always connected with the occurrence of dangers which are commonly called mining hazards. A special case of such threat is a seismic hazard which frequently occurs in many underground mines. Seismic hazard is the hardest detectable and predictable of natural hazards and in this respect it is comparable to an earthquake. More and more advanced seismic and seismoacoustic monitoring systems allow a better understanding rock mass processes and definition of seismic hazard 
prediction methods. Accuracy of so far created methods is however far from perfect. Complexity of seismic processes and big disproportion between the number of low-energy seismic events and the number of high-energy phenomena (e.g. > 10^4J) causes the statistical techniques to be insufficient to predict seismic hazard. Therefore, it is essential to search for new opportunities of better hazard prediction, also using machine learning methods. In seismic hazard assessment data clustering techniques can be 
applied (Lesniak A., Isakow Z.: Space-time clustering of seismic events and hazard assessment in the Zabrze-Bielszowice coal mine, Poland. Int. Journal of Rock Mechanics and Mining Sciences, 46(5), 2009, 918-928), and for prediction of seismic tremors artificial neural networks are used (Kabiesz, J.: Effect of the form of data on the quality of mine tremors hazard forecasting using neural networks. Geotechnical and Geological Engineering, 24(5), 2005, 1131-1147). In the majority of applications, the results obtained by mentioned methods are reported in the form of two states which are interpreted as 'hazardous' and 'non-hazardous'. Unbalanced distribution of positive ('hazardous state') and negative ('non-hazardous state') examples is a serious problem in seismic hazard prediction. Currently used methods are still insufficient to achieve good sensitivity and specificity of predictions. In the paper 
(Bukowska M.: The probability of rockburst occurrence in the Upper Silesian Coal Basin area dependent on natural mining conditions. Journal of Mining Sciences, 42(6), 2006, 570-577) a number of factors having an effect on seismic hazard occurrence was proposed, among other factors, the occurrence of tremors with energy > 10^4J was listed. The task of seismic prediction can be defined in different ways, but the main aim of all seismic hazard assessment methods is to predict (with given precision relating to time and 
date) of increased seismic activity which can cause a rockburst. In the data set each row contains a summary statement about seismic activity in the rock mass within one shift (8 hours). If decision attribute has the value 1, then in the next shift any seismic bump with an energy higher than 10^4 J was registered. That task of hazards prediction bases on the relationship between the energy of recorded tremors and seismoacoustic activity with the possibility of rockburst occurrence. Hence, such hazard prognosis is not connected with accurate rockburst prediction. Moreover, with the information about the possibility of hazardous situation occurrence, an appropriate supervision service can reduce a risk of rockburst (e.g. by distressing shooting) or withdraw workers from the threatened area. Good prediction of increased seismic activity is therefore a matter of great practical importance. The presented data set is characterized by unbalanced distribution of positive and negative examples. In the data set there 
are only 170 positive examples representing class 1. 


* Attribute Information:

1. seismic: result of shift seismic hazard assessment in the mine working obtained by the seismic 
method (a - lack of hazard, b - low hazard, c - high hazard, d - danger state); 
2. seismoacoustic: result of shift seismic hazard assessment in the mine working obtained by the 
seismoacoustic method; 
3. shift: information about type of a shift (W - coal-getting, N -preparation shift); 
4. genergy: seismic energy recorded within previous shift by the most active geophone (GMax) out of 
geophones monitoring the longwall; 
5. gpuls: a number of pulses recorded within previous shift by GMax; 
6. gdenergy: a deviation of energy recorded within previous shift by GMax from average energy recorded 
during eight previous shifts; 
7. gdpuls: a deviation of a number of pulses recorded within previous shift by GMax from average number 
of pulses recorded during eight previous shifts; 
8. ghazard: result of shift seismic hazard assessment in the mine working obtained by the 
seismoacoustic method based on registration coming form GMax only; 
9. nbumps: the number of seismic bumps recorded within previous shift; 
10. nbumps2: the number of seismic bumps (in energy range [10^2,10^3)) registered within previous shift; 
11. nbumps3: the number of seismic bumps (in energy range [10^3,10^4)) registered within previous shift; 
12. nbumps4: the number of seismic bumps (in energy range [10^4,10^5)) registered within previous shift; 
13. nbumps5: the number of seismic bumps (in energy range [10^5,10^6)) registered within the last shift; 
14. nbumps6: the number of seismic bumps (in energy range [10^6,10^7)) registered within previous shift; 
15. nbumps7: the number of seismic bumps (in energy range [10^7,10^8)) registered within previous shift; 
16. nbumps89: the number of seismic bumps (in energy range [10^8,10^10)) registered within previous shift; 
17. energy: total energy of seismic bumps registered within previous shift; 
18. maxenergy: the maximum energy of the seismic bumps registered within previous shift; 
19. class: the decision attribute - '1' means that high energy seismic bump occurred in the next shift 
('hazardous state'), '0' means that no high energy seismic bumps occurred in the next shift 
('non-hazardous state').


