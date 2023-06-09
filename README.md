# Histogram and Histogram Equalization of an image
## Aim
To obtain a histogram for finding the frequency of pixels in an Image with pixel values ranging from 0 to 255. Also write the code using OpenCV to perform histogram equalization.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import cv package.
### Step2:
Read images and use calcHist .
### Step3:
Display histogram equalization 
### Step4:
Use equilaizeHist .
### Step5:
Close the program.
## Program:
```
# Developed By:J.Archana priya
# Register Number:212221230007
```
```
import cv2
import matplotlib.pyplot as plt
```
# Write your code to find the histogram of gray scale image and color image channels.
```
gimage = cv2.imread("cbw.webp")
cimage = cv2.imread(cc.jpg",-1)
cv2.imshow("Gray Image",gimage)
cv2.imshow("Colour Image",cimage)
cv2.waitKey(0)
cv2.destroyAllWindows()




hist = cv2.calcHist([gimage],[0],None,[256],[0,256])
hist1 = cv2.calcHist([cimage],[1],None,[256],[0,256])
import cv2
import matplotlib.pyplot as plt
gimage = cv2.imread("cbw.webp")
cimage = cv2.imread("Documents/Sem4/DIP/Exp4/cc.jpg")
plt.imshow(cimage)
plt.show()
plt.imshow(gimage)
plt.show()
```
# Display the histogram of gray scale image and any one channel histogram from color image
```
plt.figure()
plt.title("Histogram")
plt.xlabel("greyscale value")
plt.ylabel("pixel count")
plt.stem(hist)
plt.show()
```
# Write the code to perform histogram equalization of the image. 
```
img = cv2.imread('cbw.webp', cv2.IMREAD_GRAYSCALE)
   equalized_img = cv2.equalizeHist(img)
    cv2.imshow('Original Image', img)
    cv2.imshow('Equalized Image', equalized_img)
    cv2.waitKey(0)
    cv2.destroyAllWindows()

```
## Output:
### Input Grayscale Image and Color Image
![op1](https://user-images.githubusercontent.com/93427594/231226890-ed6c2a38-702c-4cc7-8048-0d75d1aa4a19.png)
![op2](https://user-images.githubusercontent.com/93427594/231226934-26e07a9f-b375-41e4-8ec3-15ef5fe40859.png)

### Histogram of Grayscale Image and any channel of Color Image
![op3](https://user-images.githubusercontent.com/93427594/231227066-a73164d9-3a31-4571-85d4-c9170188f4d1.png)
![op4](https://user-images.githubusercontent.com/93427594/231228653-8aead152-e2b9-4c25-853c-74802b3837e4.png)

### Histogram Equalization of Grayscale Image
![Screenshot (403)](https://user-images.githubusercontent.com/93427594/231227498-587850d3-3471-4004-914c-b581bcbcc698.png)
![Screenshot (404)](https://user-images.githubusercontent.com/93427594/231227532-ae1ee96f-94a9-4cfb-887b-54ef019e414a.png)


## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
