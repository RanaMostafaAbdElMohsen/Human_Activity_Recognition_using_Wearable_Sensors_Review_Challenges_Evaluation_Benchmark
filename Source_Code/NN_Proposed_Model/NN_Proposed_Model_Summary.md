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

| LOSO          | NN Accuracy          | NN KFolds  |
| ------------- |:--------------------:|:----------:|
| MHealth       | 100.0%               |   96.60%   |
| USCHAD        | 99.85%               |   71.55%   |
| UTDMHAD1_1s   | 100.0%               |   46.07%   |
| UTDMHAD2_1s   | 100.0%               |   77.70%   |
| WHARF         | 99.33%               |   55.13%   |
| WISDM         | 99.90%               |   68.37%   |

- With Respect to SNOW DataSet:

| SNOW          | NN Accuracy   | NN KFolds |
| ------------- |:-------------:|:---------:|
| MHealth       | 100.0%        |   99.88%  |
| USCHAD        | 99.75%        |   92.13%  |
| UTDMHAD1_1s   | 100.0%        |   71.03%  |
| UTDMHAD2_1s   | 100.0%        |   87.97%  |
| WHARF         | 98.51%        |   74.47%  |
| WISDM         | 99.78%        |   97.19%  |
 
- With Respect to LOTO DataSet:

| LOTO          | NN Accuracy          | NN KFolds |
| ------------- |:--------------------:|:----------|
| MHealth       | 100.0%               |  93.87%   |
| USCHAD        | 99.13%               |  88.85%   |
| UTDMHAD1_1s   | 99.92%               |  71.09%   |
| UTDMHAD2_1s   | 100.0%               |  87.87%   |
| WHARF         | 98.55%               |  71.29%   |
| WISDM         | 99.95%               |  77.54%   |

- With Respect to FNOW DataSet:

| FNOW          | NN Accuracy          | NN KFolds |
| ------------- |:--------------------:|:---------:|
| MHealth       | 100.0%               |   99.55%  |
| USCHAD        | 99.85%               |   91.05%  |
| UTDMHAD1_1s   | 100.0%               |   70.29%  |
| UTDMHAD2_1s   | 100.0%               |   89.12%  |
| WHARF         | 99.53%               |   69.27%  |
| WISDM         | 99.20%               |   95.80%  |

