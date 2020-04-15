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

| LOSO          | NN_Overlapping       | NN KFolds  | NN proposed |  CNN proposed  1|  CNN proporsed 2| Another Arch  |
| ------------- |:--------------------:|:----------:|:-----------:|:---------------:|:---------------:|:-------------:|
| MHealth       | 100.0%               |   96.60%   |	99.88%    |   99.76%        |   99.53%		  |	   99.41%     |
| USCHAD        | 99.85%               |   71.55%   |   91.80%	  |   92.10%        |   91.61%        |    91.70%     |
| UTDMHAD1_1s   | 100.0%               |   46.07%   |   64.90%    |   65.70%        |   64.74%        |    63.69%     |
| UTDMHAD2_1s   | 100.0%               |   77.70%   |   81.38%    |   83.78%        |   81.38%        |    80.05%     |
| WHARF         | 99.33%               |   55.13%   |   68.94%    |   68.54%        |   70.03%        |    70.97%     |
| WISDM         | 99.90%               |   68.37%   |   94.53%    |   95.13%        |   94.03%        |    94.52%     |

- With Respect to SNOW DataSet:

| SNOW          | NN_Overlapping|  NN KFolds| NN proposed |   CNN proposed 1|  CNN proporsed 2 | Another Arch  |
| ------------- |:-------------:|:---------:|:-----------:|:--------------: |:----------------:|:-------------:|
| MHealth       | 100.0%        |   99.88%  | 99.53%      |     99.76%      |     99.76%       |    99.05%     |
| USCHAD        | 99.75%        |   92.13%  | 90.96%      |     91.76%      |     92.26%       |    91.89%     |
| UTDMHAD1_1s   | 100.0%        |   71.03%  | 64.98%      |     64.50%      |     62.73%       |    62.81%     |
| UTDMHAD2_1s   | 100.0%        |   87.97%  | 81.91%      |     81.65%      |     81.65%       |    82.71%     |
| WHARF         | 98.51%        |   74.47%  | 70.73%      |     66.98%      |     68.23%       |    71.12%     |
| WISDM         | 99.78%        |   97.19%  | 94.68%      |     95.13%      |     94.69%       |    95.10%     | 
 
- With Respect to LOTO DataSet:

| LOTO          | NN_Overlapping       | NN KFolds | NN proposed |  CNN proposed 1|  CNN proporsed 2| Another Arch  |
| ------------- |:--------------------:|:----------|:-----------:|:--------------:|:---------------:|:-------------:|
| MHealth       | 100.0%               |  93.87%   |  99.76%     |    99.76%      |   99.53%        |   99.41%      |          
| USCHAD        | 99.13%               |  88.85%   |  91.12%     |    91.89%      |   92.10%        |   91.86%      |
| UTDMHAD1_1s   | 99.92%               |  71.09%   |  67.71%     |    66.67%      |   64.02%        |   64.66%      |
| UTDMHAD2_1s   | 100.0%               |  87.87%   |  85.11%     |    81.12%      |   79.26%        |   82.71%      |
| WHARF         | 98.55%               |  71.29%   |  69.80%     |    69.56%      |   70.42%        |   73.63%      |
| WISDM         | 99.95%               |  77.54%   |  94.51%     |    94.99%      |   94.65%        |   94.80%      |

- With Respect to FNOW DataSet:

| FNOW          | NN_Overlapping       | NN KFolds | NN proposed |  CNN proposed 1|   CNN proporsed 2| Another Arch  |
| ------------- |:--------------------:|:---------:|:-----------:|:--------------:|:----------------:|:-------------:|
| MHealth       | 100.0%               |   99.55%  |  99.55%     |     99.32%     |   99.32%         |    97.73%     |
| USCHAD        | 99.85%               |   91.05%  |  89.24%     |     89.24%     |   89.66%         |    89.12%     |
| UTDMHAD1_1s   | 100.0%               |   70.29%  |  62.28%     |     60.36%     |   60.80%         |    61.09%     |
| UTDMHAD2_1s   | 100.0%               |   89.12%  |  78.43%     |     77.45%     |   79.90%         |    81.86%     |
| WHARF         | 99.53%               |   69.27%  |  63.33%     |     65.02%     |   62.34%         |    66.15%     |
| WISDM         | 99.20%               |   95.80%  |  91.96%     |     92.68%     |   91.90%         |    93.34%     |

