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

| LOSO          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 99.85%               | 
| UTDMHAD1_1s   | 99.05%               |
| UTDMHAD2_1s   | 99.56%               |
| WHARF         | 94.19%               | 
| WISDM         | 99.90%               |

- With Respect to SNOW DataSet:

| SNOW          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 99.75%               | 
| UTDMHAD1_1s   | 96.79%               |
| UTDMHAD2_1s   | 98.86%               |
| WHARF         | 93.99%               | 
| WISDM         | 99.78%               |
 
- With Respect to LOTO DataSet:

| LOTO          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 98.61%               | 
| UTDMHAD1_1s   | 96.90%               |
| UTDMHAD2_1s   | 99.91%               |
| WHARF         | 95.63%               | 
| WISDM         | 99.95%               |

- With Respect to FNOW DataSet:

| FNOW          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 100.0%               |
| USCHAD        | 98.85%               | 
| UTDMHAD1_1s   | 99.61%               |
| UTDMHAD2_1s   | 100.0%               |
| WHARF         | 95.01%               | 
| WISDM         | 99.20%               |

