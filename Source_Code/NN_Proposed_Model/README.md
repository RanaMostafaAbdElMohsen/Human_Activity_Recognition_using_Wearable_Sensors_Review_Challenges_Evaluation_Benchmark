# Neural Networks Proposed Architecture 
- Added on Contribution

## Summary
  
#### Features Extraction
There are 6 important features mentioned in Catal paper added 9 new feature:
1. Average-A(3)
2. Standard Deviation-SD(3)
3. Average Absolute Diff. AAD(3)
4. Average Resultant Acceleration ARA(1)
5. Time Between Peaks TBP
6. Binned Distribution
7. Mean
8. Max
9. Min
10. kurtosis
11. interquartile range
12. Skew
13. Area
14. Square Area
15. Median

#### Approach
15 Features + Neural Network Approach

3 Hidden layers :
128 Neurons
64 Neurons
32 Neurons

#### Paper Accuracies Obtained with Implementation Existing in Repo
- With Respect to LOSO DataSet:

| LOSO          |  NN proposed 1  |   NN proposed 2   |
|---------------|:---------------:|:-----------------:|
| MHealth       |   99.76%        |      100%         |
| USCHAD        |   92.17%        |      92.60%       |
| UTDMHAD1_1s   |   66.18%        |      67.15%       |
| UTDMHAD2_1s   |   83.51%        |      84.31%       |
| WHARF         |   74.73%        |      73.63%       |
| WISDM         |   97.24%        |      97.47%       |


- With Respect to LOTO DataSet:

| LOTO          |  NN proposed 1  |   NN proposed 2   |
|---------------|:---------------:|:-----------------:|
| MHealth       |   100%          |      99.76%       |
| USCHAD        |   92.13%        |      91.58%       |
| UTDMHAD1_1s   |   68.51%        |      65.22%       |
| UTDMHAD2_1s   |   83.51%        |      84.84%       |
| WHARF         |   75.04%        |      74.73%       |
| WISDM         |   97.50%        |      96.05%       |



- With Respect to SNOW DataSet:

| SNOW          |  NN proposed 1  |   NN proposed 2   |
|---------------|:---------------:|:-----------------:|
| MHealth       |   100%          |      100%         |
| USCHAD        |   92.72%        |      91.83%       |
| UTDMHAD1_1s   |   65.70%        |      66.51%       |
| UTDMHAD2_1s   |   85.64%        |      82.71%       |
| WHARF         |   74.24%        |      74.47%       |
| WISDM         |   95.57%        |      97.18%       |



- With Respect to FNOW DataSet:

| FNOW          |  NN proposed 1  |   NN proposed 2   |
|---------------|:---------------:|:-----------------:|
| MHealth       |   100%          |      100%         |
| USCHAD        |   89.72%        |      90.38%       |
| UTDMHAD1_1s   |   62.13%        |      61.83%       |
| UTDMHAD2_1s   |   82.84%        |      82.35%       |
| WHARF         |   69.82%        |      67.84%       |
| WISDM         |   95.45%        |      94.73%       |






- For Opportunity Dataset:

	- NN_Proposed_1  : 86.24%
	- NN_Proposed_2  : 85.78%

