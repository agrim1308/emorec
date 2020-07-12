# Emotion recognition using facial expressions
This project is 2020 summer project of brain and cognitive society ,Science and Technlogy council , **IIT Kanpur**. 
As the name suggests it is meant for leveraging the computer with the ability of classifying seven basic emotions using the facial expressions of 
humans.The seven basic emotions we're gonna classify are:

* Happy 
* Sad
* Angry
* Disgust
* Fear
* Surprise
* Contempt

## Dataset
We used the extended cohn kanade (CK+) dataset which can be found [here](https://www.kaggle.com/shawon10/ckplus)

## Reference Paper
The reference paper we used is [this](https://drive.google.com/file/d/1qMUhEFLUEuJlHO5SKjULNYfSS25ZSw4a/view) reasearch paper published on springer.

## Preprocessing
We performed the following preprocessing methods:

* [Face alignment]()
* [Face cropping]()
* [Data normalization]()
* [Data augmentation]()

## CNN model
We will be making a Sequential [model]() comprising of using two convolutional layers (conv2D), two MaxPooling2D layers , a Flatten layer followed by a output Dense layer with softmax activation , with adam optimizer and categorical crossentropy loss.

## Evaluation
We have evaluated our model on three different cropping methods:

* Cropping with background
* Cropping without background
* Cropping without forehead

Also we varied the neuron number of hidden dense layer as 0, 256, 512, 1024.
And we performed a ten fold [cross validation]() on our model keeping the cropping method fixed (without background) but varying the neuron number.

## Code
The link to the whole code is [here](https://github.com/Av-hash/EmoRec/blob/master/Emotion_Recognition_project_(1)_.ipynb).

## Results
The results of various evaluation methods we used are illustrated in this table :

### Cropping without background

|No. of neurons     |Training accuracy   |Validation accuracy   |
|---|---|---|
|0   |   |   |   
|256  |   |   |     
|512   |   |   |      
|1024   |   |   | 

### Cropping without forehead

|No. of neurons     |Training accuracy   |Validation accuracy   |
|---|---|---|
|0   |   |   |   
|256  |   |   |     
|512   |   |   |      
|1024   |   |   | 

### Cropping with background

|No. of neurons     |Training accuracy   |Validation accuracy   |
|---|---|---|
|0   |   |   |   
|256  |   |   |     
|512   |   |   |      
<<<<<<< HEAD
|1024   |   |   | 
=======
|1024   |   |   | 
>>>>>>> f235c395182547bef436f45d6206cfb541ad0620
