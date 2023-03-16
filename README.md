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
### Developed By: pragatheesvaran AB
### Register Number: 212221240039
i) #To Read,display the image
```
import cv2
import matplotlib.pyplot as plt
from google.colab.patches import cv2_imshow
I = cv2.imread('ford.jpg',1)
cv2_imshow(I)  
```
ii) #To write the image
```
I = cv2.imread('ford.jpg',1)
cv2_imshow(I)
cv2.imwrite('a1.jpg',I)

```
iii) #Find the shape of the Image
```python3
import cv2
color=cv2.imread('bi.jpg',1)
print(color.shape)



```
iv) #To access rows and columns

```python3
import cv2
import random
I= cv2.imread('lab.webp',-1)
for i in range(150):
    for j in range(I.shape[1]):
        I[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2_imshow(I)
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```python3
import cv2
I= cv2.imread('bi.jpg',-1)
new = I[200:450,200:450]
I[150:400,150:400] = new
cv2_imshow(I)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

<br>![output](show.jpg)
<br>![output](gray.png)

### ii)Write the image

<br>![output](true.jpg)
<br>

### iii)Shape of the Image

<br>![output](shape.jpg)
<br>

### iv)Access rows and columns

<br>![output](blur.jpg)
<br>

### v)Cut and paste portion of image
<br>![output](cut.jpg)
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


