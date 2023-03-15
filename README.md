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
### Developed By: RAKSHITHA DEVI J
### Register Number:  212221230082
i) #To Read,display the image
```
import cv2
import matplotlib.pyplot as plt
from google.colab.patches import cv2_imshow
img1=cv2.imread("/content/f1.jpg",1)
cv2_imshow(img1)
cv2.waitKey(0)
cv2.destroyAllWindows()
  

```
ii) #To write the image
```
import cv2
import matplotlib.pyplot as plt
from google.colab.patches import cv2_imshow
A=cv2.imread("/content/f1.jpg",1)
cv2.imwrite("/content/f1.jpg",A)
cv2_imshow(A)
cv2.waitKey(0)



```
iii) #Find the shape of the Image
```
import random
import cv2
import matplotlib.pyplot as plt
from google.colab.patches import cv2_imshow
A=cv2.imread("f1.jpg",1)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2_imshow(A)
cv2.waitKey(0)



```
iv) #To access rows and columns

```
import random
import cv2
import matplotlib.pyplot as plt
from google.colab.patches import cv2_imshow
A=cv2.imread("f1.jpg",1)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2_imshow(A)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```
import cv2
import matplotlib.pyplot as plt
from google.colab.patches import cv2_imshow
A=cv2.imread("f1.jpg",1)
tag=A[140:240,165:180]
A[25:125,50:65]=tag
cv2_imshow(A)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image

![image](https://user-images.githubusercontent.com/94165326/225260866-4fb4d460-deb3-4888-b3ac-75d4c6f2e79a.png)

### ii)Write the image

![image](https://user-images.githubusercontent.com/94165326/225260985-98d13530-9cbd-484f-9736-0e69075c52aa.png)

### iii)Shape of the Image

![image](https://user-images.githubusercontent.com/94165326/225261069-348d7fb6-a95e-461c-a6ee-1b9e1fef4334.png)

### iv)Access rows and columns
![image](https://user-images.githubusercontent.com/94165326/225261146-75a01f82-6835-40ec-9d41-98a2e94cae12.png)
### v)Cut and paste portion of image
![image](https://user-images.githubusercontent.com/94165326/225261295-2cb7f079-d35e-466b-8d0e-1f7a56688914.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


