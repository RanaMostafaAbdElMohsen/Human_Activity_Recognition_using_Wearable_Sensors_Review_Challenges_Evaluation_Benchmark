# Neural Networks Proposed Architecture 
- Added on Contribution

## Summary
  
#### Features Extraction
There are 6 important features mentioned in Catal paper:
1. Average-A(3)
2. Standard Deviation-SD(3)
3. Average Absolute Diff. AAD(3)
4. Average Resultant Acceleration ARA(1)
5. Time Between Peaks TBP
6. Binned Distribution

#### Approach
Catal Feature Extraction + Neural Network Approach

3 Hidden layers :
128 Neurons
64 Neurons
32 Neurons

Accuracies were reported for only 6 activities

#### Paper Accuracies Obtained with Implementation Existing in Repo
- With Respect to LOSO DataSet:

| LOSO          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 97.68%               | 
| UTDMHAD1_1s   | 84.83%               |
| UTDMHAD2_1s   | 99.56%               |
| WHARF         | 87.68%               | 
| WISDM         | 99.90%               |

- With Respect to SNOW DataSet:

| SNOW          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 97.20%               | 
| UTDMHAD1_1s   | 95.60%               |
| UTDMHAD2_1s   | 98.86%               |
| WHARF         | 83.51%               | 
| WISDM         | 98.40%               |
 
- With Respect to LOTO DataSet:

| LOTO          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 97.76%               | 
| UTDMHAD1_1s   | 93.00%               |
| UTDMHAD2_1s   | 99.82%               |
| WHARF         | 87.26%               | 
| WISDM         | 99.56%               |

- With Respect to FNOW DataSet:

| FNOW          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 97.68%               | 
| UTDMHAD1_1s   | 92.97%               |
| UTDMHAD2_1s   | 100.0%               |
| WHARF         | 84.20%               | 
| WISDM         | 98.72%               |

