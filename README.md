# Scene_Explainer using AI
"A picture is worth a thousand words" is an idiom that conveys its meaning as 'Seeing something is better for learning than having it described'.
But what if you see something(image/scene) for the first time and your brain can't analyze what is it?

Don't worry! An automatic AI model which generators caption or explain the scene is all you need to analyze smth you see for the first time. 

This project is all about generating captions by extracting the features from the images and predicting the captions from the model.

# Dataset 
The MS COCO (Microsoft Common Objects in Context) dataset is large-scale object detection, segmentation, key-point detection, and captioning dataset. The dataset consists of 328K images. The 2014 training/validation split is 118K/5K and the test set is a subset of 41K images. The dataset has annotations for captioning: natural language descriptions of the images. 
You can download the dataset here https://cocodataset.org/#download

![Screenshot (268)](https://user-images.githubusercontent.com/52888140/162217565-f73acde7-4a84-4d71-88b4-194fd2de1143.png)


# Model Overview 
Resnet50 is used for image classification and for the extraction of features.

![Screenshot (369)](https://user-images.githubusercontent.com/52888140/162217618-65fa6e88-c790-4783-9c26-56eb8e97ab95.png)

The attention Based Mechanism is used for caption generation. I have used Bahdanau’s Attention or Local Attention. The attention mechanism is focusing on the relevant part of the image, so the decoder only uses specific parts of the image.
![Screenshot (373)](https://user-images.githubusercontent.com/52888140/162217660-b39e07fb-b614-4527-adae-85f16083bd17.png)

# Result
![Screenshot (370)](https://user-images.githubusercontent.com/52888140/162217696-9103b2af-d38a-4ab8-a907-e9f7cc4264ce.png)

![Screenshot (371)](https://user-images.githubusercontent.com/52888140/162217750-9cdd7694-5790-4ea5-a667-9c7306dbbe17.png)

![Screenshot (372)](https://user-images.githubusercontent.com/52888140/162217776-558faaad-3987-4d8c-894b-5dae6990bb53.png)


# Note :
This is a phase 1 model, as I will be improving it using transforms or GPT3 model
