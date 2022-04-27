# Histogram and Histogram Equalization of an image
## Aim
To obtain a histogram for finding the frequency of pixels in an Image with pixel values ranging from 0 to 255. Also write the code using OpenCV to perform histogram equalization.

## Software Required:
Anaconda - Python 3.7

## Algorithm: 
```
##Step1:

Import all the necessary libraries.

##Step2:

Read the images using imread() function.

##Step3:

Using calcHist() we can find the histogram of the images.

##Step4:

Using equalizeHist() we can equalize the image.

##Step5:

Using matplotlib.pyplot plot the histogram.
```
## Program:
```python
# Developed By:S.Meena.
# Register Number:212221240028
import cv2
import matplotlib.pyplot as plt

# Write your code to find the histogram of gray scale image and color image channels.
import cv2
import matplotlib.pyplot as plt
gray_image = cv2.imread("cc.jpg")
color_image = cv2.imread("gg.jpg",-1)
cv2.imshow("Gray Image",gray_image)
cv2.imshow("Colour Image",color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()





# Display the histogram of gray scale image and any one channel histogram from color image
import cv2
import matplotlib.pyplot as plt
Gray_image = cv2.imread('gg.jpeg')
plt.imshow(Gray_image)
plt.show()
hist = cv2.calcHist([Gray_image],[0],None,[256],[0,256])
plt.figure()
plt.title("Histogram")
plt.xlabel('Grayscale_value')
plt.ylabel('pixel count')
plt.stem(hist)
plt.show(




# Write the code to perform histogram equalization of the image. 

import cv2
gray_image = cv2.imread("gg.jpg",0)
cv2.imshow('grey scale image',gray_image)
equ = cv2.equalizeHist(gray_image)
cv2.imshow("Equalized Image",equ)
cv2.waitKey(0)
cv2.destroyAllWindows 






```
## Output:
### Input Grayscale Image and Color Image
![image](https://user-images.githubusercontent.com/94677128/165501820-519975b3-5426-4025-ad41-00eb3d414d19.png)
![image](https://user-images.githubusercontent.com/94677128/165501853-d38d7009-5586-4115-b02d-c8cacf270797.png)


### Histogram of Grayscale Image and any channel of Color Image
![image](https://user-images.githubusercontent.com/94677128/165501976-72d4b9ec-64a9-48ef-83e6-bc596c8cc1fc.png)
![image](https://user-images.githubusercontent.com/94677128/165502018-7e5c3d4a-98a6-48b4-92d6-2f7eb51f8cf3.png)

### Histogram Equalization of Grayscale Image
![image](https://user-images.githubusercontent.com/94677128/165502064-67e99f3b-b24e-4ac1-a86f-77af1d52d93a.png)

## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
