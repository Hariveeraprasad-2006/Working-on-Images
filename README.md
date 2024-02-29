# Working-on-Images
### Aim
 
Aim:
 
To write a python program using OpenCV to capture the image from the web camera and do the following image manipulations.
1. The image should be a plant, Tree, flower or building
2. The filename should be username.jpg
3. The image should be Converted to gray scale and HSV 
4. Display the H, S and V planes
## Software Used
Anaconda - Python 3.7
## Algorithm
## Step 1:
Use cv2.imread to read the image

## Step 2:
Use cv2.COLOR_RGB2GRAY to change the image into rgb to gray
## Step 3:
Usecv2.COLOR_RGB2HSV to change the image into rgb to hsv
## Step 4:
use cv2.split(hsv_image) to split the image.

## Step 5:
End the program.
## Program:
``` Python
### Developed By: ARIKATLA HARI VEERA PRASAD
### Register No:  212223240014
import cv2
color_image=cv2.imread("username.jpg")
cv2.imshow("colorimage",color_image)
gray_image1=cv2.cvtColor(color_image,cv2.COLOR_RGB2GRAY)
cv2.imshow("RGB2GRAY",gray_image1)
hsv_image=cv2.cvtColor(color_image,cv2.COLOR_RGB2HSV)
cv2.imshow("RGB2HSV",hsv_image)
h,s,v=cv2.split(hsv_image)
cv2.imshow("H PLANE",h)
cv2.imshow("S PLANE",s)
cv2.imshow("V PLANE",v)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# Result:
Thus the images are read and color conversion was performed between RGB To GRAY, HSV  color models successfully using the python program.
