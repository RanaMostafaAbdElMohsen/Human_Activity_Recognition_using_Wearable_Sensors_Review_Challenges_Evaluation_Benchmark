# Bevilacqua et al 2019
https://arxiv.org/pdf/1906.01935.pdf
## Summary
https://docs.google.com/document/d/1I96tZfD0pYkfr3qb4VsUtid2StrkhLovwHx70Vk2KBw/edit?usp=sharing
### About Paper

#### Background & Info
- The physical activities targeted in this paper are part of 
  the Otago Exercise Programme 
- Grouped 16 different activities into
	four categories: walk, walking balance, standing balance, and strength
	
- The chosen device for this study is Shimmer3,e returns a 
  set of six signals (three acceleration components, over the axes x, y and z, and three angular velocity components
- The sampling rate is set to 102.4 Hz for all sensors  
- The group of 19 participants consists of 7 males and 12 
  females. Participants have a mean age of 22.94±2.39, a mean height of 164.34±7.07 cm, and a mean weight of 66.78±11.92 kg	

  
#### Preprocessing
- Datset segmented into small overlapping windows of 204  
  points,  corresponding to roughly 2 seconds of movements,
  with a stride of 5 points




#### Paper Approach
- Training  Model :
	- training epochs varies from 150
		to up to 300
	- learning rate is fixed to 0.005
	- a batch size of 1024	
- evaluate the performance of model based on :
	- collect individual precision and recall scores
		for every combination of sensors and activities,
		then compute the Fscores.
	
#### Paper Model architecture

| Layer          | Params               | 
| -------------  |:--------------------:| 
| conv2d_1       | (3x5)                |
| BtachNorm      |                      |
| MaxPool        | (3x3)                | 
| conv2d_2       | (2x4)                | 
| BtachNorm      |                      |
| MaxPool        | (2x2)                |
| conv2d_3       | (2x2)                | 
| BtachNorm      |                      |
| MaxPool        | (3x2)                |
| Flatten_1      | (500)                |
| Flatten_2      | (250)                |
| dense_1        | (115)                | 



#### Paper Accuracies Obtained with Implementation Existing in Repo
- With Respect to LOSO DataSet:

| LOSO          | Bevilacqua Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 85.00%               |
| USCHAD        | ------               | 
| UTDMHAD1_1s   | ------               |
| UTDMHAD2_1s   | ------               |
| WHARF         | ------               | 
| WISDM         | ------               |

- With Respect to SNOW DataSet:

| SNOW          | Bevilacqua Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 93.11%               |
| USCHAD        | ------               | 
| UTDMHAD1_1s   | ------               |
| UTDMHAD2_1s   | ------               |
| WHARF         | ------               | 
| WISDM         | ------               |
 
- With Respect to LOTO DataSet:

| LOTO          | Bevilacqua Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 89.62%               |
| USCHAD        | ------               | 
| UTDMHAD1_1s   | ------               |
| UTDMHAD2_1s   | ------               |
| WHARF         | ------               | 
| WISDM         | ------               |

- With Respect to FNOW DataSet:

| FNOW          | Bevilacqua Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 95.96%               |
| USCHAD        | ------               | 
| UTDMHAD1_1s   | ------               |
| UTDMHAD2_1s   | ------               |
| WHARF         | ------               | 
| WISDM         | ------               |

- With Repect to HHAR Non-Overlapping Slidding Window:
   - Couldn't be trained due to Dataset size with Model

- With Repect to HHAR Overlapping Slidding Window:
	- Couldn't be trained due to Dataset size with Model

- With Repect to Opportunity:
	- 86.68%	
