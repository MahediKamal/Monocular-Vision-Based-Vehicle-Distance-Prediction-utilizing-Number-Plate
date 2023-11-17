# Demo video of the project while predicting the distance
![](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/readme%20res/f2400df5-f2a8-4f9f-b6ab-bebaa0905c90.gif)
# We have implemented 2 different method for predicting the distance based on the number plate

- Method 1: Distance prediction in respect of number size on the number plate. This methid can be devided into two main steps: <br>
  - Step 1: Object Detection (Number plate detection). We have a YoloV5 model for detecting number plate. <br>
    - Data set for traing the YoloV5 model  [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/tree/main/Data%20Set/numberPlate_train_data)
    - Trained YoloV5 model link for number plate detection. [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/Trained%20models/number_plate_model2.pt)
    - read dataset readme and model readme for details. (LINK)
  - Spet 2: Distance Prediction. This step can be sudevided into 2 steps.
    - Step 2.1: We have used image processing and BFS algorithm to calculate the pixel sixe of digits on number plate.
      - Code for calculating numbel length in pixel on number plate (LINK)
    - Step 2.2: We have Trained model for predicting distance based on the calculated pixel on step 2.1
      - We have two types trained model and both predict distance individually. We can choose any of them.
      - Model 1: CNN model.
        - data set for training the CNN model (LINK)
        - Trained CNN model (LINK)
        - CNN model structure (IMAGE)
      - Model 2: regression mode.
        - data set for training the regression model (LINK)
        - equation of the regression model (LINK)
- Method 2: Distance Prediction in respect of height and width of the number plate. This methid can be devided into two main steps:
  - Step 1: Object Detection (Number plate detection). We have a YoloV5 model for detecting number plate.
    - Data set for traing the YoloV5 model [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/tree/main/Data%20Set/numberPlate_train_data)
    - Trained YoloV5 model link for number plate detection. [LINK](https://github.com/MahediKamal/Monocular-Vision-Based-Vehicle-Distance-Prediction-utilizing-Number-Plate/blob/main/Trained%20models/number_plate_model2.pt)
    - read dataset readme and model readme for details. (LINK)
  - Spet 2: Distance Prediction. This step can be sudevided into 2 steps.
    - Step 2.1: We get the height and width of number plate from the YoloV5 model we have created to detect number plate.
    - Step 2.2: We have Trained model for predicting distance based on the calculated height and widthg on step 2.1
      - We have two types trained model and both predict distance individually. We can choose any of them.
      - Model 1: CNN model.
        - data set for training the CNN model (LINK)
        -Trained CNN model (LINK)
        - CNN model structure (IMAGE)
      - Model 2: regression mode.
        - data set for training the regression model (LINK)
        - equation of the regression model (LINK)

We have 5 types of dataset-


```
  1. still car image taken by 48 mp camera
  2. moving car back view taken by samsung galaxcy A12
  3. moving car front fiew taken by samsung galaxcy A12
  4. moving car back view taken by Iphone 13
  5. moving car front fiew taken by Iphone 13
```

We will calculate distance predicting accuracy for each of the 5 type of dataset individually.

## 1. still car image taken by 48 mp camera
### model link
### accuracy
### result image

## 2. moving car back view taken by samsung galaxcy A12
### model link
### accuracy
### result image

## 3. moving car front fiew taken by samsung galaxcy A12
### model link
### accuracy
### result image

## 4. moving car back view taken by Iphone 13
### model link
### accuracy
### result image

## 5. moving car front fiew taken by Iphone 13
### model link
### accuracy
### result image


# colab code
# work 2 - (creating a model that can detect some native vehiche of bangladesh and then compare the model with COCO model)

Our model can recognize-
```
  0. human
  1. car
  2. bus
  3. rickshaw
  4. bike
  5. cng
  6. bicycle
  7. van
  8. easybike
```

## image of the vehicles
## model link
## detection image
## coparison data
## colab code
  
