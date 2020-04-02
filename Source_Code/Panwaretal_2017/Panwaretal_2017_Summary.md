# Panwar et al. 2015
https://www.ncbi.nlm.nih.gov/pubmed/29060391

## Summary
https://docs.google.com/document/d/13RBlVf5hCFd2rVwn19_KIMjUZnaJVjm_07aRUCO_Pmg/edit?usp=sharing
### About Paper

#### Background & Info
- Paper proposed architecture to detect arm movements
- Classes : 3 Classes including :
	- Action A – Reach and retrieve an object
	- Action B – Lift cup to mouth
	- Action C – Perform pouring or (un)locking action
- wearable Shimmer 9DoF,having tri-axis accelerometer, gyroscope, and a magnetometer.	

  
#### Preprocessing
There are 3 type of preprocessing mentioned in the paper, that produce 3 different datasets:
1. Basic Preprocessing:
	- data are normalized and then resampled to fixed length i.e. 64 points 

2. Advanced Preprocessing:
	- Smoothing- Makes the model insignificant to small perturbations
	- Normalization- Transformation of all data into specific range (0 -1). 
	- Mode capturing- Removal of undesired part where no activity has occurred and extract the required signal
	- Resampling- Conversion of all data from variable size to fixed size
3. Synthetic Data


#### Paper Approach
- Training two different architectures based on preprocessing type.
- evaluate the performance of model based on three cases:
	- Cross-validation evaluation-Training and testing
		with cross-validation.
	- Inter-subject evaluation - Training with 3 subjects
		and testing with other subject
	- Hybrid evaluation- Out of 4 repetitions, Training
		with 3 sets of data taken from each subject and
		testing with remaining one set from each subject.	

#### Paper Model architecture
1- Architecture 1
| Layer          | Params               | 
| -------------  |:--------------------:| 
| conv2d_1       | (5,9,3)              |
| conv2d_2       | (5,5,3)              | 
| Max2d_1        | (2,1)                |
| Flatten_1      | (480)                |
| dense_1        | (3)                  | 

1- Architecture 2
| Layer          | Params               | 
| -------------  |:--------------------:| 
| conv2d_1       | (5,9,3)              |
| conv2d_2       | (5,7,3)              | 
| conv2d_3       | (5,5,3)              | 
| Max2d_1        | (2,1)                |
| Flatten_1      | (480)                |
| dense_1        | (3)                  | 

#### Paper Accuracies Obtained with Implementation Existing in Repo
- With Respect to LOSO DataSet:

| LOSO          | Panwar Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 09.01%               |
| USCHAD        | 14.72%               | 
| UTDMHAD1_1s   | 05.23%               |
| UTDMHAD2_1s   | 40.63%               |
| WHARF         | ------               | 
| WISDM         | ------               |

- With Respect to SNOW DataSet:

| SNOW          | Panwar Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 09.00%               |
| USCHAD        | 13.84%               | 
| UTDMHAD1_1s   | 05.22%               |
| UTDMHAD2_1s   | 51.59%               |
| WHARF         | ------               | 
| WISDM         | ------               |
 
- With Respect to LOTO DataSet:

| LOTO          | Panwar Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 09.02%               |
| USCHAD        | 13.85%               | 
| UTDMHAD1_1s   | 05.24%               |
| UTDMHAD2_1s   | 50.00%               |
| WHARF         | ------               | 
| WISDM         | ------               |

- With Respect to FNOW DataSet:

| FNOW          | Panwar Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 08.99%               |
| USCHAD        | 13.50%               | 
| UTDMHAD1_1s   | 05.27%               |
| UTDMHAD2_1s   | 48.04%               |
| WHARF         | ------               | 
| WISDM         | ------               |

- With Repect to HHAR Non-Overlapping Slidding Window:
Couldn't be trained due to Dataset size with Model

- With Repect to HHAR Overlapping Slidding Window: 18.80%

- With Repect to Opportunity: 84.22%
 