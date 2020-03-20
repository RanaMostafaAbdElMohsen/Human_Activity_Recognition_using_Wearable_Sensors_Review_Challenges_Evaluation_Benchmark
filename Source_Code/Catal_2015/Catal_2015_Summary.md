# Catal 2015 Paper 
- Doi : [Catal 2015 Paper](https://doi.org/10.1016/j.asoc.2015.01.025)

## Summary

### About Paper

#### Background & Info
- Sensor : Accelerometer 
- Classes : 12 Classes including walking, jogging, upstairs, downstairs & standing, etc...
- Acceleraton recorded in 3 axis:
  - x-axis : horizontal motion of leg
  - y-axis : upward / downward motion
  - z-axis : forward acceleration
- 2 Activity Modes:
  - Ascending -> small peaks for y-axis and z-axis
  - Descending -> small peaks reported for y-axis
  - As summary we are interested in y-axis and z-axis
  
#### Features Extraction
There are 6 important features mentioned in the paper
1- Average-A(3)
2- Standard Deviation-SD(3)
3- Average Absolute Diff. AAD(3)
4- Average Resultant Acceleration ARA(1)
5- Time Between Peaks TBP
6- Binned Distribution

#### Paper Approach
Majority Voting Between 3 classical classifiers
1- J48 Decision Tree Algorithm
2- Logistic Regression
3- MLP
Accuracies were reported for only 6 activities

#### Paper Accuracies Obtained with Implementation Existing in Repo
- With Respect to LOSO DataSet:

| LOSO          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 95.87%               |
| USCHAD        | 74.62%               | 
| UTDMHAD1_1s   | 31.98%               |
| UTDMHAD2_1s   | 73.67%               |
| WHARF         | 49.69%               | 
| WISDM         | 73.86%               |
 
