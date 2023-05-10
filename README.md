## Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
## Step1:
Import necessary packages

## Step2:
Create a empty window and add text in it

## Step3:
Create a structuring element

## Step4:
Do the operation

## Step5:
Do the operation
## Program:
## Developed By:B.Pavizhi
## Register No:212221230077
## Import the necessary packages
```

import cv2
import numpy as np
import matplotlib.pyplot as plt

```

## Create the Text using cv2.putText
```

img1=np.zeros((100,660),dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX = 3
cv2.putText(img1,'ezhil',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1,'gray')
plt.axis('off')
```


## Create the structuring element
```

kernel=np.ones((5,5),np.uint8)


```
## Erode the image
```

image_erode1=cv2.erode(img1,kernel)
plt.imshow(image_erode1,'gray')
plt.axis('off')

```

## Dilate the image
```
image_dilatel=cv2.dilate(img1,kernel)
plt.imshow(image_dilatel,'gray')
plt.axis('off')
```
## Output:

## Display the input Image
![](./1.png)

## Display the Eroded Image
![](./2.png)

## Display the Dilated Image
![](./3.png)
## Result
Thus the generated text image is eroded and dilated using python and OpenCV.