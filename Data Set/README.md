# About dataset

```
	Dataset file name -> numberPlate_train_data{
	        Dataset for trainng a model that can detect number plate
		Dataset is formated acording to YoloV5 trainig.
		
	}

	Dataset file name -> Distance Vs Length-Width (Iphone13pro){
		Data set has 3 colums - dx ,dy , distance
		This data set is used to train model that can predict distance based on the number plate width and height
		Data set depends on the camera specification. with the change of camera data set will also change. So we will have different models for different camera.
		For this dataset we have used Iphone13pro (12 MP camera)
		we have taken a video of a running car, then split the video into image frame. Then used these frames for calculating width heigh-distance-dataset
		
	}
		
	Dataset file name -> Distance Vs Pixel (samsungGalaxyA12_48mpStill_image){
		Data set has 2 colums - pixel , distance
		data for distance prediction based on pixel number
		Data set depends on the camera specification. with the change of camera data set will also change. So we will have different models for different camera.
		For this dataset we have used Samsung Galaxy A12 (setting was 48 MP camera)
	}
		


```
