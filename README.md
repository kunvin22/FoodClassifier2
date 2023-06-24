# Food Classifier
*to get model:go to master branch of github instead of main branch
A ai model that classifies food between chip, cookies and ice cream using Jetson-inferences resnet-18 model

![image](https://github.com/kunvin22/FoodClassifier2/assets/56424209/ae4b7361-117a-4272-8f53-c35b94408e2b)

## The Algorithm
=
This project is a jetson inferences resnet18 model which dataset consists of foods like chips, cookies and icecream. When it is run, it uses the imagenet.py program with the model to determine the instrument family of an inputted image.
![image](https://github.com/kunvin22/FoodClassifier2/assets/56424209/a56720d1-3832-4370-bcf5-d453e731c926)

## Running this project

1. Make 2 variables NET=models/foods, DATASET=data/foodclass
2. run imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --$Dataset/labels.txt $DATASET/test/chips/120_chips.jpg result.jpg
    $DATASET/test/chips/120_chips.jpg = to the file you want to input
    result.jpg = name of the file you want to output
3. open your laptops terminal
4. scp <nanousername>@192.168.55.1:/home/<nanousername>/myProject/classification/result.jpg C:\Users\<hostusername>\Desktop
5. open C:\Users\<hostusername>\Desktop on files and find result.jpg

[[View a video explanation here](video link)](https://youtu.be/2ytgJoQKFKQ)https://youtu.be/2ytgJoQKFKQ
