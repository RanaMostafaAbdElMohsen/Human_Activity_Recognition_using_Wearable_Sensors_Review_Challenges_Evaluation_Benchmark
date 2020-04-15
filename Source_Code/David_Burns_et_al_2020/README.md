# David M. Burns et al 2020
https://arxiv.org/pdf/2001.05517.pdf
## Summary

### About Paper

#### Background & Info
- Datset Used: MHEALTH, WISDM, and SPAR
- These data sets encompass a combination of activities of daily living, exercise activity, and physiotherapy activities.
- Class balance is approximately equal within each and there is minimal missing data.

  
#### Preprocessing
-  The WISDM and MHEALTH data was resampled to 50 Hz, using cubic interpolation.
-  A four second sliding window was utilized for the MHEALTH and SPAR data sets, and a ten second window was utilized for WISDM 
   for consistency
-  An overlap ratio of 0.8 was used in the sliding window segmentation as a data augmentation strategy.
-  only the smart watch data from the WISDM data set, because the smart watch and mobile phone data were not synchronized during 
   data collection   



#### Paper Approach
Proposed 3 different models
- Impersonal Fully Convolutional Network (FCN)(Implemented)

	- Training  Model :
		- a learning rate of 0.001		
		- Optomizer Adam
		- number of epoch 150
- Personalized Feature Classifier
	Three personalized feature classifiers: personalized engineered features (PEF), personalized deep features (PDF), and
	personalized triplet network (PTN) were implemented and compared for activity classification performance. Inference
	is achieved in each of these models by comparing a subject’s embedded test segments to labeled reference embeddings
	specific to the subject. 	
- Hardware:
	Experiments were carried out locally on a computer with two NVIDIA Titan V GPUs for hardware acceleration.		

		

	
- evaluate the performance of model based on :
	- evaluated using 5-fold cross-validation grouping folds by subject
	
	
#### Paper Model architecture

FCN 

| Layer          | Params               | 
| -------------  |:--------------------:| 
| Conv1D         |  (128,8,1)           |
| BN,RELU,Dropout|                      |
| Conv1D         | (256,5,1)            | 
| BN,RELU,Dropout|                      |
| conv1D         | (128,3,1)            |
|BN,RELU,Dropout |                      |
|GAP             |                      |
|L2 Norm         |                      |
| fullyconnected | (num_classes)        | 




#### Paper Accuracies Obtained with Implementation Existing in Repo

- With Respect to LOSO DataSet :

| LOSO          | David Burns Model Accuracy | 
| ------------- |:--------------------:	     | 
| MHealth       | 91.78%                     |
| USCHAD        | ------                     |  
| UTDMHAD1_1s   | 30.33%                     |
| UTDMHAD2_1s   | 64.96%                     |
| WHARF         | 49.87%                     | 
| WISDM         | ------                     |



- With Respect to SNOW DataSet :

| SNOW          | David Burns Model Accuracy | 
| ------------- |:--------------------:	     | 
| MHealth       | 95.54%                     |
| USCHAD        | ------                     |  
| UTDMHAD1_1s   | 33.39%                     |
| UTDMHAD2_1s   | 69.05%                     |
| WHARF         | 62.40%                     | 
| WISDM         | 98.82%                     |


- With Respect to LOTO DataSet :

| LOTO          | David Burns Model Accuracy | 
| ------------- |:--------------------:	     | 
| MHealth       | 89.77%                     |
| USCHAD        | ------                     |  
| UTDMHAD1_1s   | 33.64%                     |
| UTDMHAD2_1s   | 69.02%                     |
| WHARF         | 61.59%                     | 
| WISDM         | ------                     |



- With Respect to FNOW DataSet :

| FNOW          | David Burns Model Accuracy | 
| ------------- |:--------------------:	     | 
| MHealth       | 93.65%                     |
| USCHAD        | ------                     |  
| UTDMHAD1_1s   | 26.46%                     |
| UTDMHAD2_1s   | 65.55%                     |
| WHARF         | 57.70%                     | 
| WISDM         | 96.46%                     |

