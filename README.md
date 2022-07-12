# Trffic-rule-prediction-ML-Project

# About Project

There are several different types of traffic signs like speed limits, no entry, traffic signals, turn left or right, children crossing, no passing of heavy vehicles, etc. Traffic signs classification is the process of identifying which class a traffic sign belongs to.

# About Dataset 

The dataset contains more than 50,000 images of different traffic signs. It is further classified into 43 different classes. The dataset is quite varying, some of the classes have many images while some classes have few images. The size of the dataset is around 300 MB. 
We use Kaggle Dataset of train our Machine learning Model . 

[Dataset of Project](https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign)

# Architecture our Model 

1. 2 Conv2D layer (filter=32, kernel_size=(5,5), activation=”relu”)<br/>
2. MaxPool2D layer ( pool_size=(2,2))<br/>
3. Dropout layer (rate=0.25)<br/>
4. 2 Conv2D layer (filter=64, kernel_size=(3,3), activation=”relu”)<br/>
5. MaxPool2D layer ( pool_size=(2,2))<br/>
6. Dropout layer (rate=0.25)<br/>
7. Flatten layer to squeeze the layers into 1 dimension <br/>
8. Dense Fully connected layer (256 nodes, activation=”relu”) <br/>
9. Dropout layer (rate=0.5)<br/>
10. Dense layer (43 nodes, activation=”softmax”) <br/>

