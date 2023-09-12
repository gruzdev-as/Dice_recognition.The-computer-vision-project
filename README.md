<p float="center">
<img src="/GIFs/1.gif" width="25%" height="25%"/>
<img src="/GIFs/6.gif" width="25%" height="25%"/>
</p>

# Dice-recognition.-The-computer-vision-project

A set of Jupyter notebooks for training various computer vision models for classifying and recognizing dice of various configurations and values on the sides of a die. 

## Installation and Usage 

I strongly recommend you to use the Google Colab environment. All the notebooks were originally exported from the Google Colab. In case if you want to train models locally, I'd like to suggest using Python Virtual environment:

```sh
python -m venv /path/to/new/virtual/environment
```
I do not attach the requirement.txt file here, because for different notebooks different packages and libraries are required. 

## Brief description

During the project several tasks were completed. Each notebook contains one exact task solved. In order of increasing difficulty:

1. *DiceTypeRecognition.ipynb* contains the process of training the ResNet50 model for solving a classification task of recognition Dice types. The following steps were completed and described:
    - Data uploading and preparation
    - ResNet50 transfer learning preparation
    - Training process
    - Model evaluation
    - Model saving

In the end, the following results were achieved. 

![output](https://github.com/gruzdev-as/Dice-recognition.-The-computer-vision-project/assets/75714678/c5d0d8eb-c4a1-4efc-94d4-43bce568bf66)

The dataset is used: https://www.kaggle.com/datasets/ucffool/dice-d4-d6-d8-d10-d12-d20-images

2. *D6DiceValueRecognition.ipynb* contains the process of training YOLOV5 and YOLOV8 models by ultralytics for solving an object-detection task. The task was to detect values on the top side of a d6-die in the "dot-notation". Two models were trained and compared with use both self-made imges and videos. The following results were achieved and described in detail inside the notebook:


<p float="center">
<img src="/GIFs/5.gif" width="25%" height="25%"/>
<img src="/GIFs/6.gif" width="25%" height="25%"/>
<img src="/GIFs/7.gif" width="25%" height="25%"/>
</p>

Based on the results, I can conclude that the newest model perform way better than the old one. despite this fact it still has difficulties with recognition the difference between "5" and "6". In my humble opinion it's conneted with the fact that the dataset images differ from the images and videos I've made myself. Perhaps, the model is overfitted a little bit. Due to that facts I decided to make a task more complicated and try to create my own dataset 

The dataset is used: https://public.roboflow.com/object-detection/dice/2

3. *D6DiceValueRecognitionWithNumbers.ipynb* contains the process of training a YOLOV8 model by ultralytics for solving an object-detection task similar to the previous one. This time dices had numbers on them instead of just dots. I didn't find the dataset in the net, so, I've made it myself. The dataset is used with the description and the methodology: https://universe.roboflow.com/test-pxksd/d6-dice-with-numbers-on-the-sides. The following results were achieved and described in detail inside the notebook:

![output1](https://github.com/gruzdev-as/Dice-recognition.-The-computer-vision-project/assets/75714678/5ef2a57c-cab9-4da9-b980-919edde28d24)

<p float="left">
<img src="/GIFs/1.gif" width="25%" height="25%"/>
<img src="/GIFs/2.gif" width="25%" height="25%"/>
<img src="/GIFs/3.gif" width="25%" height="25%"/>
</p>

## Conclusion 

While working on the project, I not only acquired basic skills in data processing for computer vision, training and evaluating computer vision models for classification and object recognition problems, but also made a small contribution to the developing data science community. I hope that the work I have done will help not only me to become more confident and competent in an area of interest to me, but will also be useful for other aspiring data engineers and data scientists.

