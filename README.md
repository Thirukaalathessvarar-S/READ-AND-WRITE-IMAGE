# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By: Thirukaalathessvarar S
### Register Number: 212222230161
i) #To Read,display the image
```
 import cv2
color_img=cv2.imread('DIPexp1.jpg',1)
cv2.imshow('212222230161',color_img)
cv2.waitKey(0)
```
ii) #To write the image
```
import cv2
color_img=cv2.imread('DIPexp1.jpg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212222230161',color_img)
cv2.waitKey(0)
```
iii) #Find the shape of the Image
```
import cv2
import random
color_img=cv2.imread('DIPexp1.jpg',1)
print(color_img.shape)
```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('DIPexp1.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222230161',color_img)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
color_image=cv2.imread('DIPexp1.jpg',-1)
tag=color_image[300:400,300:400]
color_image[50:150,50:150]=tag
cv2.imshow('212222230161',color_image)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image
![DIP_exp_output](https://github.com/Thirukaalathessvarar-S/READ-AND-WRITE-IMAGE/assets/121166390/fa912c5c-47fd-4bae-bbe7-45263780f3ea)

### ii)Write the image
![dip_real_output2](https://github.com/Thirukaalathessvarar-S/READ-AND-WRITE-IMAGE/assets/121166390/0716a9ae-39fb-4c73-ba7c-443875828d01)



### iii)Shape of the Image
![dip_output3](https://github.com/Thirukaalathessvarar-S/READ-AND-WRITE-IMAGE/assets/121166390/e7926682-40de-403a-ba46-36e359c7dbba)


### iv)Access rows and columns
![dip_real_ouptut](https://github.com/Thirukaalathessvarar-S/READ-AND-WRITE-IMAGE/assets/121166390/588b85a4-cabe-4cf5-9cf7-e93e58f593c2)


### v)Cut and paste portion of image
![dip_realoutput5](https://github.com/Thirukaalathessvarar-S/READ-AND-WRITE-IMAGE/assets/121166390/b797b077-f570-4f55-92fd-a4b281aac099)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
