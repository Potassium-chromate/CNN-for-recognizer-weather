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
### process
1. load pictures and resize to (300,300,3)
2. randomized the order of pictures and labels by using 'sklearn.utils.shuffle'
