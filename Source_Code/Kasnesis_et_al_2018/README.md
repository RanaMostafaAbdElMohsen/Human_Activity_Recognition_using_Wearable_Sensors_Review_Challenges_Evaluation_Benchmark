# Kasnesis et al 2018
https://arxiv.org/abs/1811.00170
## Summary

### About Paper

#### Background & Info
- Datset Used: The UCI-HAR, WISDM, OPPORTUNITY

  
#### Preprocessing
-  LINEAR INTERPOLATION
-  SCALING AND NORMALIZATION  

- SEGMENTATION
	- a sliding window with an overlap rate of 50% was used 
	  to segment the data collected by motion sensors.
	- For the WISDM and UCI-HAR dataset, the length of the  
	   sliding window is 128.
	- The length of the sliding window for the OPPORTUNITY 
	   dataset is chosen to be 24   



#### Paper Approach
- Training  Model :
	- a learning rate of 0.001		
	- Optomizer Adam
	- number of epoch 200
	- Batch size 192
- The model training and classification were on a PC that has an E5-2620 Xeon CPU with 2.10 GHz, 64GB RAM and an NVIDIA QUADRO 
   P5000 graphics card with 16 GB memory. And the PC is equipped with an Ubuntu operating system with 64 bits.
	
- evaluate the performance of model based on :
	- F-measure, it takes into account
	both the precision and the recall of each class to compute 	the score and can evaluate the model better than the precision
	
#### Paper Model architecture

| Layer          | Params               | 
| -------------  |:--------------------:| 
| LSTM           | 64                   |
| LSTM           | 64                   |
| conv1D         | (64Fx1x5x2S)         | 
| MaxPooling     | (1x2x2S)             |
| conv1D         | (128Fx1x3x2S)        |
|GAP             |                      |
|BatchNorm       |                      |
| fullyconnected | (num_classes)        | 




#### Paper Accuracies Obtained with Implementation Existing in Repo

- With Respect to LOSO DataSet :

| LOSO          | Kasnesis Model Accuracy  | 
| ------------- |:--------------------:	   | 
| MHealth       | 93.81%                   |
| USCHAD        | ------                   | 
| UTDMHAD1_1s   | 32.60%                   |
| UTDMHAD2_1s   | 71.02%                   |
| WHARF         | 65.13%                   | 
| WISDM         | ------                   |



- With Respect to SNOW DataSet :

| SNOW          | Kasnesis Model Accuracy  | 
| ------------- |:--------------------:	   | 
| MHealth       | 99.96%                   |
| USCHAD        | ------                   | 
| UTDMHAD1_1s   | 56.41%                   |
| UTDMHAD2_1s   | 84.62%                   |
| WHARF         | 87.45%                   | 
| WISDM         | 99.65%                   |


- With Respect to LOTO DataSet :

| LOTO          | Kasnesis Model Accuracy  | 
| ------------- |:--------------------:	   | 
| MHealth       | 87.89%                   |
| USCHAD        | 90.94%                   | 
| UTDMHAD1_1s   | 53.97%                   |
| UTDMHAD2_1s   | 82.44%                   |
| WHARF         | 83.47%                   | 
| WISDM         | 91.02%                   |



- With Respect to FNOW DataSet :

| FNOW          | Kasnesis Model Accuracy  | 
| ------------- |:--------------------:	   | 
| MHealth       | 99.70%                   |
| USCHAD        | 91.55%                   | 
| UTDMHAD1_1s   | 45.99%                   |
| UTDMHAD2_1s   | 79.76%                   |
| WHARF         | 78.49%                   | 
| WISDM         | 99.06%                   |

