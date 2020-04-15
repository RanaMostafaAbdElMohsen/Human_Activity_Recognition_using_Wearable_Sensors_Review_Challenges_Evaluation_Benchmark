# Lingjuan Lyu al 2017
https://www.researchgate.net/publication/320883605_Privacy-Preserving_Collaborative_Deep_Learning_with_Application_to_Human_Activity_Recognition?enrichId=rgreq-11191b898a62b6b37d73081740a9304c-XXX&enrichSource=Y292ZXJQYWdlOzMyMDg4MzYwNTtBUzo1NTk0OTA0MDM5MTM3MjhAMTUxMDQwNDMxNTMxOQ%3D%3D&el=1_x_3&_esc=publicationCoverPdf
## Summary

### About Paper

#### Background & Info
- Datset Used: The UCI-HAR, Mobile health dataset

  
#### Preprocessing
-  UCI-HAR
	- The sensor signals were pre-processed by applying noise filters 
	- n sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window)
- 	Mobile health dataset
	- sampled in fixed-width sliding windows of 128 readings/window





#### Paper Approach

	
#### Paper Model architecture

| Layer          | Params               | 
| -------------  |:--------------------:| 
| LSTM           | 18/28                |
| LSTM           | 18/28                |
| conv1D         | (30,5)               |
| conv1D         | (40,10)              |
|conv1D          | (50,15)              |
|conv1D          | (60,20)              |
|Max pooling     |                      |
| fullyconnected | (num_classes)        | 




#### Paper Accuracies Obtained with Implementation Existing in Repo

- With Respect to LOSO DataSet :

| LOSO          | Lingjuan Model Accuracy  | 
| ------------- |:--------------------:	   | 
| MHealth       | 92.05%                   |
| USCHAD        | ------                   | 
| UTDMHAD1_1s   | 36.73%                   |
| UTDMHAD2_1s   | 74.77%                   |
| WHARF         | 70.95%                   | 
| WISDM         | ------                   |



- With Respect to SNOW DataSet :

| SNOW          | Lingjuan Model Accuracy  | 
| ------------- |:--------------------:	   | 
| MHealth       | 99.77%                   |
| USCHAD        | ------                   | 
| UTDMHAD1_1s   | 61.53%                   |
| UTDMHAD2_1s   | 86.13%                   |
| WHARF         | 88.99%                   | 
| WISDM         | 99.47%                   |


- With Respect to LOTO DataSet :

| LOTO          | Lingjuan Model Accuracy  | 
| ------------- |:--------------------:	   | 
| MHealth       | 89.17%                   |
| USCHAD        | ------                   | 
| UTDMHAD1_1s   | 57.10%                   |
| UTDMHAD2_1s   | 83.64%                   |
| WHARF         | 85.07%                   | 
| WISDM         | 89.19%                   |



- With Respect to FNOW DataSet :

| FNOW          | Lingjuan Model Accuracy  | 
| ------------- |:--------------------:	   | 
| MHealth       | 99.33%                   |
| USCHAD        | 89.92%                   | 
| UTDMHAD1_1s   | 52.27%                   |
| UTDMHAD2_1s   | 80.21%                   |
| WHARF         | 83.29%                   | 
| WISDM         | 98.46%                   |

