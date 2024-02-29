# Working-on-Images
### Aim
 
Aim:
 
To write a python program using OpenCV to convert image to gray and hsv. display the  H,S,V.
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
# Output:
# Orignal Image:
![Screenshot 2024-02-29 100433](https://github.com/Hariveeraprasad-2006/Working-on-Images/assets/145049988/267835aa-00dc-43be-b734-7f6846bc2d10)
# Gray Image:
![Screenshot 2024-02-29 100416](https://github.com/Hariveeraprasad-2006/Working-on-Images/assets/145049988/a29a6cc7-7e1d-47e4-a6e3-f5dc87181cb4)
# HSV Image:
![Screenshot 2024-02-29 100359](https://github.com/Hariveeraprasad-2006/Working-on-Images/assets/145049988/a5812dcd-8a88-4441-81b6-0cc3ecac0bc4)
# H Image:
![Screenshot 2024-02-29 100341](https://github.com/Hariveeraprasad-2006/Working-on-Images/assets/145049988/74349092-9c94-430e-ab74-b2ab39bfb055)
# S Image:
![Screenshot 2024-02-29 100321](https://github.com/Hariveeraprasad-2006/Working-on-Images/assets/145049988/e10458b3-0e93-4ee0-99b1-290b4b7a5763)
# V Image:
![Screenshot 2024-02-29 100257](https://github.com/Hariveeraprasad-2006/Working-on-Images/assets/145049988/e1937010-e88c-4dcc-b854-c233b099553b)
# Result:
Thus the images are read and color conversion was performed between RGB To GRAY, HSV  color models successfully using the python program.
