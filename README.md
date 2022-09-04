# Low-cost-Road-damage-detection-and-classification-using-accelerometer-sensor-and-machine-lear
classification of different damages of road using 3-D accelerometer data
  Road condition monitoring is a challenging problem in the field of road transportation infrastructure all over the world.
 A zone in bad condition may damage the vehicles on it, endanger the drivers, and even cause accidents, So city municipalities have spent millions of dollars to maintain and repair these roadways. 
 This is due to lack of comprehensive and up-to-date information on degrading road conditions is only exacerbating the already inefficient, expensive and labor-expensive methods associated with road maintenance and repair.
 Nowadays sensors embedded smartphone and accelerometers is widely used in monitoring road surfaces ,because of  it’s guaranteeing an adequate maintenance by road managers can be achieved via having inexpensive, sufficient and accurate information concerning road infrastructure quality.
![image](https://user-images.githubusercontent.com/110971636/188305954-87bea28b-f543-461a-87f6-5a7ddcdea8f0.png)




I’ll prefer ADXL335 OR ADXL345 for the following reasons:
Along with some advantages as mention above, the range of this instrument is more than enough to conduct our project.
The acceleration data  can be accessed either by Secure Digital (SD) card or using USB cable connected to our personal computer (PC).
Pack consists of AURDINO board which is  used to connect accelerometer to PC and SD card.
Programming Code of accelerometer can be modified by connecting sensor to laptop using AURDINO board.
 Hyperlink of source code and details of connection and program of sensor:-
     https://mechstuff.com/adxl335-accelerometer-arduino-tutorial-with-calibration/
![image](https://user-images.githubusercontent.com/110971636/188305990-0b8970e4-4f01-466f-96e3-559de37e48f7.png)
 
 
 Cleaning and labelling raw data in excel:-![image](https://user-images.githubusercontent.com/110971636/188306012-75ba62c7-5f2f-41fb-8e9d-bb59af2e07b7.png)

 Accelerometer sensor or smartphone is mounted on test drive vehicle along with GPS sensor (if we want to know the location of damaged surface).
  Collect data from both sensors along the selected length of road and save it to the external SD card or to the PC.
  The collected data is stored in CSV format, so load it to the excel spread sheet and fill null values with mean and remove unwanted data columns.
  Make labels corresponding to sequence of accelerometer data by creating new column. Then our data is ready for classification.
![image](https://user-images.githubusercontent.com/110971636/188306001-6b04c034-8c06-4bf4-b319-eb21398bd402.png)



First we have to check the z-axis accelerometer readings corresponding to different defects of road manually and according to that we can classify them based on changes in vertical accelerations.
   Let’s look into how each type of road anomaly affects the z-axis accelerometer data graphically.
   For digital output the best indicator is that z -acceleration tends to stay at gravity acceleration which is +10 m/sq-sec Using this information can be concluded that vehicle crosses normal road will have its z-acceleration relatively stays at +10 m/sq-sec. Any rise or fall from this value is the indicator of road anomaly.
![image](https://user-images.githubusercontent.com/110971636/188306038-47874651-0124-4f77-8d52-547a6da6849b.png)

