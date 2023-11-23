# Demo video of the project while predicting the distance
![](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/readme%20res/f2400df5-f2a8-4f9f-b6ab-bebaa0905c90.gif)
# We have implemented 2 different method for predicting the distance based on the number plate

- ### `Method 1: Distance prediction in respect of number size on the number plate. This method can be devided into two main steps: `
  - #### `Step 1:` Object Detection (Number plate detection). We have a YoloV5 model for detecting number plate. <br>
    - Data set for traing the YoloV5 model  [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/tree/main/Data%20Set/numberPlate_train_data)
    - Trained YoloV5 model link for number plate detection. [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/Trained%20models/number_plate_model2.pt)
  - #### `Spet 2:` Distance Prediction. This step can be sudevided into 2 steps.
    - ##### Step 2.1: We have used image processing and BFS algorithm to calculate the pixel sixe of digits on number plate.
      - Code for calculating numbel length in pixel on number plate (LINK)
    - ##### Step 2.2: We have Trained model for predicting distance based on the calculated pixel on step 2.1
      - We have two types trained model and both predict distance individually. We can choose any of them.
      - Model 1: CNN model.
        - data set for training the CNN model [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/Data%20Set/Distance%20Vs%20Pixel%20(samsungGalaxyA12_48mpStill_image).csv)
        - CNN model structure:
          - ![...](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/readme%20res/ann1.png)
      - Model 2: regression mode.
        - data set for training the regression model [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/Data%20Set/Distance%20Vs%20Pixel%20(samsungGalaxyA12_48mpStill_image).csv)
        - equation of the regression model is of power 4
- ### `Method 2: Distance Prediction in respect of height and width of the number plate. This methid can be devided into two main steps:`
  -  #### `Step 1:` Object Detection (Number plate detection). We have a YoloV5 model for detecting number plate.
     - Data set for traing the YoloV5 model [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/tree/main/Data%20Set/numberPlate_train_data)
     - Trained YoloV5 model link for number plate detection. [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/Trained%20models/number_plate_model2.pt)
  -  #### `Spet 2:` Distance Prediction. This step can be sudevided into 2 steps.
     - ##### Step 2.1: We get the height and width of number plate from the YoloV5 model we have created to detect number plate.
     - ##### Step 2.2: We have Trained model for predicting distance based on the calculated height and widthg on step 2.1
       - We have two types trained model and both predict distance individually. We can choose any of them.
       - Model 1: CNN model.
         - data set for training the CNN model [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/Data%20Set/Distance%20Vs%20Length-Width%20(Iphone13pro).csv)
         - CNN model structure:
           - ![...](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/readme%20res/ann2.png)
       - Model 2: regression mode.
         - data set for training the regression model [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/Data%20Set/Distance%20Vs%20Length-Width%20(Iphone13pro).csv)
         - equation of the regression model is of power 4



