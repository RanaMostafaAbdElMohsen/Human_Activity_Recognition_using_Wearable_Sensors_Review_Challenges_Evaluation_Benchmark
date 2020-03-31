# HHAR UCI Datasey
https://archive.ics.uci.edu/ml/datasets/Heterogeneity+Activity+Recognition
## Summary

### About DataSet

#### Background & Info
- The data is split into 4 files in total divided by device (phone or watch) and sensor (gyroscope and accelerometer).
- The files for phones are: Phones_accelerometer.csv, Phones_gyroscope.csv for the accelerometer and gyroscope respectively, and for the Watch_accelerometer.csv, Watch_gyroscope.csv for the accelerometer and gyroscope as well.

- Activities: ‘Biking’, ‘Sitting’, ‘Standing’, ‘Walking’, ‘Stair Up’ and ‘Stair down’.
- Sensors: Two embedded sensors, i.e., Accelerometer and Gyroscope sampled at the highest frequency possible by the device
- Devices: 4 smartwatches (2 LG watches, 2 Samsung Galaxy Gears) 8 smartphones (2 Samsung Galaxy S3 mini, 2 Samsung Galaxy S3, 2 LG Nexus 4, 2 Samsung Galaxy S+)
- Recordings: 9 users currently named: a,b,c,d,e,f,g,h,i consistently across all files.

#### CSV file Structure
-'Index', 'Arrival_Time', 'Creation_Time', 'x', 'y', 'z', 'User', 'Model', 'Device', 'gt'
- And the columns have the following values:
- Index: 		is the row number.
- Arrival_Time:	The time the measurement arrived to the sensing application
- Creation_Time	The timestamp the OS attaches to the sample
- X,y,z		The values provided by the sensor for the three axes, X,y,z
- User:		The user this sample originates from, the users are named a to i.
- Model:		The phone/watch model this sample originates from
- Device:		The specific device this sample is from. They are prefixed with the model name and then the number, e.g., nexus4_1 or nexus4_2.
- Gt:		The activity the user was performing: bike sit, stand, walk, stairsup, stairsdown and null

  
#### Preprocessing
- Data Used Mobile Phone sensor reading
- Data Loaded for both files Phones_accelerometer.csv,Phones_gyroscope.csv
- The both files are merged into one file
- We apply sliding window overlaping and non Overlapping techniques
- DataSet Shape for Non-Overalpping (102050, 128, 6) indicating number of Data, Window Size , Number of sensors
- DataSet Shape for Overalpping (1306247, 10, 6) indicating number of Data, Window Size , Number of sensors
- DataSet is then stroed as crompressed file NPZ

#### Proceesed Dataset
https://drive.google.com/open?id=11gDiVVr2U34idEz-ukXkWKFavZw84chJ





