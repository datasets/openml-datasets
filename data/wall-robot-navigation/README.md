The resources for this dataset can be found at https://www.openml.org/d/1497

Author: Ananda Freire, Marcus Veloso and Guilherme Barreto     
Source: [UCI](https://archive.ics.uci.edu/ml/datasets/Wall-Following+Robot+Navigation+Data) - 2010  
Please cite: [UCI](https://archive.ics.uci.edu/ml/citation_policy.html)

Wall-Following Robot Navigation Data Data Set  
The data were collected as the SCITOS G5 robot navigates through the room following the wall in a clockwise direction, for 4 rounds, using 24 ultrasound sensors arranged circularly around its 'waist'.

The data consists of raw values of the measurements of all 24 ultrasound sensors and the corresponding class label. Sensor readings are sampled at a rate of 9 samples per second.

The class labels are:  
1. Move-Forward,  
2. Slight-Right-Turn,  
3. Sharp-Right-Turn,  
4. Slight-Left-Turn  

It is worth mentioning that the 24 ultrasound readings and the simplified distances were collected at the same time step, so each file has the same number of rows (one for each sampling time step). 

The wall-following task and data gathering were designed to test the hypothesis that this apparently simple navigation task is indeed a non-linearly separable classification task. Thus, linear classifiers, such as the Perceptron network, are not able to learn the task and command the robot around the room without collisions. Nonlinear neural classifiers, such as the MLP network, are able to learn the task and command the robot successfully without collisions. 

### Attribute Information:

1. US1: ultrasound sensor at the front of the robot (reference angle: 180°) 
2. US2: ultrasound reading (reference angle: -165°)
3. US3: ultrasound reading (reference angle: -150°)
4. US4: ultrasound reading (reference angle: -135°)
5. US5: ultrasound reading (reference angle: -120°)
6. US6: ultrasound reading (reference angle: -105°)
7. US7: ultrasound reading (reference angle: -90°)
8. US8: ultrasound reading (reference angle: -75°) 
9. US9: ultrasound reading (reference angle: -60°) 
10. US10: ultrasound reading (reference angle: -45°)
11. US11: ultrasound reading (reference angle: -30°) 
12. US12: ultrasound reading (reference angle: -15°)
13. US13: reading of ultrasound sensor situated at the back of the robot (reference angle: 0°) 
14. US14: ultrasound reading (reference angle: 15°)
15. US15: ultrasound reading (reference angle: 30°)
16. US16: ultrasound reading (reference angle: 45°)
17. US17: ultrasound reading (reference angle: 60°)
18. US18: ultrasound reading (reference angle: 75°)
19. US19: ultrasound reading (reference angle: 90°)
20. US20: ultrasound reading (reference angle: 105°)
21. US21: ultrasound reading (reference angle: 120°)
22. US22: ultrasound reading (reference angle: 135°)
23. US23: ultrasound reading (reference angle: 150°)
24. US24: ultrasound reading (reference angle: 165°)


### Relevant Papers

Ananda L. Freire, Guilherme A. Barreto, Marcus Veloso and Antonio T. Varela (2009), 'Short-Term Memory Mechanisms in Neural Network Learning of Robot Navigation Tasks: A Case Study'. Proceedings of the 6th Latin American Robotics Symposium (LARS'2009), pages 1-6 
