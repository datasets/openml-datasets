The resources for this dataset can be found at https://www.openml.org/d/42

Author: R.S. Michalski and R.L. Chilausky (Donors: Ming Tan & Jeff Schlimmer)  
Source: [UCI](https://archive.ics.uci.edu/ml/datasets/Soybean+(Large)) - 1988  
Please cite: R.S. Michalski and R.L. Chilausky "Learning by Being Told and Learning from Examples: An Experimental Comparison of the Two Methods of Knowledge Acquisition in the Context of Developing an Expert System for Soybean Disease Diagnosis", International Journal of Policy Analysis and Information Systems, Vol. 4, No. 2, 1980.  

Large Soybean Database  
This is the large soybean database from the UCI repository, with its training and test database combined into a single file. 

There are 19 classes, only the first 15 of which have been used in prior work. The folklore seems to be that the last four classes are unjustified by the data since they have so few examples. There are 35 categorical attributes, some nominal and some ordered. The value 'dna' means does not apply. The values for attributes are encoded numerically, with the first value encoded as "0,'' the second as "1,'' and so forth. An unknown value is encoded as "?''.

### Attribute Information

1. date: april,may,june,july,august,september,october,?. 
2. plant-stand: normal,lt-normal,?. 
3. precip: lt-norm,norm,gt-norm,?. 
4. temp: lt-norm,norm,gt-norm,?. 
5. hail: yes,no,?. 
6. crop-hist: diff-lst-year,same-lst-yr,same-lst-two-yrs, 
same-lst-sev-yrs,?. 
7. area-damaged: scattered,low-areas,upper-areas,whole-field,?. 
8. severity: minor,pot-severe,severe,?. 
9. seed-tmt: none,fungicide,other,?. 
10. germination: 90-100%,80-89%,lt-80%,?. 
11. plant-growth: norm,abnorm,?. 
12. leaves: norm,abnorm. 
13. leafspots-halo: absent,yellow-halos,no-yellow-halos,?. 
14. leafspots-marg: w-s-marg,no-w-s-marg,dna,?. 
15. leafspot-size: lt-1/8,gt-1/8,dna,?. 
16. leaf-shread: absent,present,?. 
17. leaf-malf: absent,present,?. 
18. leaf-mild: absent,upper-surf,lower-surf,?. 
19. stem: norm,abnorm,?. 
20. lodging: yes,no,?. 
21. stem-cankers: absent,below-soil,above-soil,above-sec-nde,?. 
22. canker-lesion: dna,brown,dk-brown-blk,tan,?. 
23. fruiting-bodies: absent,present,?. 
24. external decay: absent,firm-and-dry,watery,?. 
25. mycelium: absent,present,?. 
26. int-discolor: none,brown,black,?. 
27. sclerotia: absent,present,?. 
28. fruit-pods: norm,diseased,few-present,dna,?. 
29. fruit spots: absent,colored,brown-w/blk-specks,distort,dna,?. 
30. seed: norm,abnorm,?. 
31. mold-growth: absent,present,?. 
32. seed-discolor: absent,present,?. 
33. seed-size: norm,lt-norm,?. 
34. shriveling: absent,present,?. 
35. roots: norm,rotted,galls-cysts,?.

### Classes 

-- 19 Classes = {diaporthe-stem-canker, charcoal-rot, rhizoctonia-root-rot, phytophthora-rot, brown-stem-rot, powdery-mildew, downy-mildew, brown-spot, bacterial-blight, bacterial-pustule, purple-seed-stain, anthracnose, phyllosticta-leaf-spot, alternarialeaf-spot, frog-eye-leaf-spot, diaporthe-pod-&-stem-blight, cyst-nematode, 2-4-d-injury, herbicide-injury} 

### Revelant papers

Tan, M., & Eshelman, L. (1988). Using weighted networks to represent classification knowledge in noisy domains. Proceedings of the Fifth International Conference on Machine Learning (pp. 121-134). Ann Arbor, Michigan: Morgan Kaufmann. 

Fisher,D.H. & Schlimmer,J.C. (1988). Concept Simplification and Predictive Accuracy. Proceedings of the Fifth International Conference on Machine Learning (pp. 22-28). Ann Arbor, Michigan: Morgan Kaufmann. 

