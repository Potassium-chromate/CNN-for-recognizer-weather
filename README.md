# CNN-for-recognizer-weather
## 1. Purposes
Utilize CNN to classify the type of weather present in the image
## 2.Target
We use CNN to to classify the type of weather present in the image.There will be a training set and test set. Training set include 1147 RGB pictures and a few gray picture. The training set include 75 RGB pictures.
### One-hot encoding for the label  
`0:cloudy
1:rain
2:shine
3:sunrise`
## 3.Method
### CNN structure
![Alt Text](https://github.com/Potassium-chromate/CNN-for-recognizer-weather/blob/main/Picture/Model%20structure.png)
### Process
1. Load pictures and resize to (300,300,3)
2. Additional augmentation for the picture  
   `rotate 45 and 60 degrees`  
   `flipped`
4. Randomized the order of pictures and labels by using `sklearn.utils.shuffle`
5. Start training
6. Generate a chart to evaluate the performance of the model

## 4.Result
### Accuracy curve
![Alt Text](https://github.com/Potassium-chromate/CNN-for-recognizer-weather/blob/main/Picture/Accuracy%20curve.png)
### Loss curve
![Alt Text](https://github.com/Potassium-chromate/CNN-for-recognizer-weather/blob/main/Picture/Loss%20curve.png)
### Train confusion
![Alt Text](https://github.com/Potassium-chromate/CNN-for-recognizer-weather/blob/main/Picture/train_confusion.png)
### Test confusion
![Alt Text](https://github.com/Potassium-chromate/CNN-for-recognizer-weather/blob/main/Picture/test_confusion.png)
