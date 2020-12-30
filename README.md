# maskdetection
***
This project is about detecting whether a person is wearing a mask or not in the camera.

I used a face mask dataset from the below git location which contains set of images with and without mask.

https://github.com/prajnasb/observations/tree/master/experiements/data

After getting the face of the person in front of the camera, the image will be passed through a cascade classifier(haarcascade_frontalface_default.xml). This classifier will provide the region of interest of the face. 

After that, we will resize the region of interest into a 224x224 and pass it to a pre-trained CNN, it will give us the probability of the person wearing a mask or not as an output.

