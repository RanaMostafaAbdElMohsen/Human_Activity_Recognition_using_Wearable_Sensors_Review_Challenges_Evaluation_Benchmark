# HaChoi 2016 Paper 
- Doi : [HaChoi 2016 Paper](10.1109/IJCNN.2016.7727224)

## Summary

### About Paper

#### Background & Info
- Sensor : Accelerometer 
- Classes : 12 Classes including walking, jogging, upstairs, downstairs & standing, etc...
- Acceleraton recorded in 3 axis:
  - x-axis : horizontal motion of leg
  - y-axis : upward / downward motion
  - z-axis : forward acceleration

#### Paper Approach
- Full weight sharing vs Partial weight sharing
- Zero padding convolution subsampling
- CNN Model :
  - CNN_pf
  - CNN_pff
- CNN_pff is implemented in this paper 
- CNN_pff employs 3 different convolution kernel sets in lower layer which is appled to mode 1 and mode 2

#### Paper Accuracies Obtained with Implementation Existing in Repo
- With Respect to LOSO DataSet:

| LOSO          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 76.18%               |
| USCHAD        | -------              | 
| UTDMHAD1_1s   | -------              |
| UTDMHAD2_1s   | -------              |
| WHARF         | -------              | 
| WISDM         | -------              |

- With Respect to SNOW DataSet:

| SNOW          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 76.66%               |
| USCHAD        | -------              | 
| UTDMHAD1_1s   | -------              |
| UTDMHAD2_1s   | -------              |
| WHARF         | -------              | 
| WISDM         | -------              |
 
- With Respect to LOTO DataSet:

| LOTO          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 84.77%               |
| USCHAD        | -------              | 
| UTDMHAD1_1s   | -------              |
| UTDMHAD2_1s   | -------              |
| WHARF         | -------              | 
| WISDM         | -------              |

- With Respect to LOTO DataSet:

| FNOW          | Catal Model Accuracy | 
| ------------- |:--------------------:| 
| MHealth       | 79.85%               |
| USCHAD        | -------              | 
| UTDMHAD1_1s   | -------              |
| UTDMHAD2_1s   | -------              |
| WHARF         | -------              | 
| WISDM         | -------              |