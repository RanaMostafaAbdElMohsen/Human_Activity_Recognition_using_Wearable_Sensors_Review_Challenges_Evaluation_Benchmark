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

#### Paper Accuracies Obtained with Implementation Existing in Repo
- With Respect to LOSO DataSet:

| LOSO          | NN Accuracy          | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 99.85%               | 
| UTDMHAD1_1s   | 100.0%               |
| UTDMHAD2_1s   | 100.0%               |
| WHARF         | 99.33%               | 
| WISDM         | 99.90%               |

- With Respect to SNOW DataSet:

| SNOW          | NN Accuracy          | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 99.75%               | 
| UTDMHAD1_1s   | 100.0%               |
| UTDMHAD2_1s   | 100.0%               |
| WHARF         | 98.51%               | 
| WISDM         | 99.78%               |
 
- With Respect to LOTO DataSet:

| LOTO          | NN Accuracy          | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 99.13%               | 
| UTDMHAD1_1s   | 99.92%               |
| UTDMHAD2_1s   | 100.0%               |
| WHARF         | 98.55%               | 
| WISDM         | 99.95%               |

- With Respect to FNOW DataSet:

| FNOW          | NN Accuracy          | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 99.85%               | 
| UTDMHAD1_1s   | 100.0%               |
| UTDMHAD2_1s   | 100.0%               |
| WHARF         | 99.53%               | 
| WISDM         | 99.20%               |

