# Jian Sun et al 2018
https://www.hindawi.com/journals/js/2018/8580959/
## Summary
https://docs.google.com/document/d/19ORHFY05gM035UpxD-7SD3C9j29edp-UfUTOz3Oifb8/edit?usp=sharing
### About Paper

#### Background & Info
- Datset Used: OPPORTUNITY
- OPPORTUNITY dataset are extremely imbalanced, the NULL 
  Class accounts for more than 70% of all the data
- The convolutional neural network assumes that the
   inputs and outputs of the model are independent from each
   other,thus, some time information must be included in the input data. Long short-term memory (LSTM) network has been proposed to solve this problem. Use ELM network as fully connected classifier
- OPPORTUNITY activity recognition dataset is composed of a
   set of complex human natural activities collected in an environment where rich sensors are installed
	
- consider the on-body sensors, including inertial 
   measurement units and 3-axis accelerometers
- Each sensor channel is treated as an individual channel, a
	total of 113 channels. The sampling frequency of these
	sensors is 30 Hz.
- OPPORTUNITY dataset contains gestures and postures
- 18-class classification problem;

  
#### Preprocessing
- used 0 to fill in missing values of the sensor data
- each sensor channel was normalized to interval 0, 1
- used a fixed-length sliding window to segment data
- The length of the window is 500 ms and the step size is 
   250 ms




#### Paper Approach
- Training  Model :
	- a learning rate of 0.001		
	- a decay factor of 0.9
	
- evaluate the performance of model based on :
	- F-measure, it takes into account
	both the precision and the recall of each class to compute 	the score and can evaluate the model better than the precision
	
#### Paper Model architecture

| Layer          | Params               | 
| -------------  |:--------------------:| 
| conv2d_1       | (5x1)                |
| conv2d_2       | (5x1)                |
| conv2d_3       | (5x1)                | 
| conv2d_4       | (5x1)                |
| LSTM           |  128                 |
| LSTM           |  128                 |
| ELM/ fullyconn | (num_classes)        | 




#### Paper Accuracies Obtained with Implementation Existing in Repo

- With Respect to LOSO DataSet with ELM:

| LOSO          | Jian  Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 81.57%               |
| USCHAD        | ------               | 
| UTDMHAD1_1s   | 19.37%               |
| UTDMHAD2_1s   | 50.90%               |
| WHARF         | 50.52%               | 
| WISDM         | ------               |

- With Respect to LOSO DataSet without ELM:

| LOSO          | Jian Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 78.48%               |
| USCHAD        | 59.13%               | 
| UTDMHAD1_1s   | 18.97%               |
| UTDMHAD2_1s   | 51.17%               |
| WHARF         | 49.39%               | 
| WISDM         | ------               |

- With Respect to SNOW DataSet:

| SNOW          | Jian Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | ------               |
| USCHAD        | ------               | 
| UTDMHAD1_1s   | ------               |
| UTDMHAD2_1s   | ------               |
| WHARF         | ------               | 
| WISDM         | ------               |
 
- With Respect to LOTO DataSet:

| LOTO          | Jian Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | ------               |
| USCHAD        | ------               | 
| UTDMHAD1_1s   | ------               |
| UTDMHAD2_1s   | ------               |
| WHARF         | ------               | 
| WISDM         | ------               |

- With Respect to FNOW DataSet:

| FNOW          | Jian Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | ------               |
| USCHAD        | ------               | 
| UTDMHAD1_1s   | ------               |
| UTDMHAD2_1s   | ------               |
| WHARF         | ------               | 
| WISDM         | ------               |