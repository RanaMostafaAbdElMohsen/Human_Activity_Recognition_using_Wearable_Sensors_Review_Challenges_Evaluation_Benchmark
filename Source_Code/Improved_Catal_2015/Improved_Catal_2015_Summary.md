# Improved Catal 2015 Paper 
- Added on Contribution

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
There are 6 important features mentioned in Catal paper:
1. Average-A(3)
2. Standard Deviation-SD(3)
3. Average Absolute Diff. AAD(3)
4. Average Resultant Acceleration ARA(1)
5. Time Between Peaks TBP
6. Binned Distribution

#### Improved Approach
Majority Voting Between 3 classical classifiers
1. J48 Decision Tree Algorithm
2. Logistic Regression
3. SVM
Accuracies were reported for only 6 activities

#### Paper Accuracies Obtained with Implementation Existing in Repo
- With Respect to LOSO DataSet:

| LOSO          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 96.64%               |
| USCHAD        | 75.64%               | 
| UTDMHAD1_1s   | 49.10%               |
| UTDMHAD2_1s   | 74.92%               |
| WHARF         | 49.69%               | 
| WISDM         | 80.10%               |

- With Respect to SNOW DataSet:

| SNOW          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 90.92%               | 
| UTDMHAD1_1s   | 51.10%               |
| UTDMHAD2_1s   | 82.80%               |
| WHARF         | 68.89%               | 
| WISDM         | 90.08%               |
 
- With Respect to LOTO DataSet:

| LOTO          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 95.16%               |
| USCHAD        | 87.31%               | 
| UTDMHAD1_1s   | 49.60%               |
| UTDMHAD2_1s   | 82.33%               |
| WHARF         | 65.49%               | 
| WISDM         | 80.15%               |

- With Respect to FNOW DataSet:

| FNOW          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 99.77%               |
| USCHAD        | 88.92%               | 
| UTDMHAD1_1s   | 49.01%               |
| UTDMHAD2_1s   | 79.18%               |
| WHARF         | 62.71%               | 
| WISDM         | 88.47%               |

