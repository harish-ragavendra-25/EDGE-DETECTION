# EDGE-DETECTION
## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import all the necessary modules for the program.
### Step2:
Load a image using imread() from cv2 module.
### Step3:
Convert the image to grayscale
### Step4:
Using Sobel operator from cv2,detect the edges of the image.
### Step5:
Using Laplacian operator from cv2,detect the edges of the image and Using Canny operator from cv2,detect the edges of the image.
## PROGRAM:
```
DEVELOPED BY: HARISH RAGAVENDRA S
REGISTER NUMBER: 212222230045
```
```
import cv2
import matplotlib.pyplot as plt
```
```
img=cv2.imread("dipt_img.jpg",0)
gray=cv2.cvtColor(img,cv2.COLOR_GRAY2RGB)
gray = cv2.GaussianBlur(gray,(3,3),0)
```
```
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.imshow(sobelx,cmap='gray')
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
```
```
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.imshow(sobelx,cmap='gray')
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
```
```
sobelxy = cv2.Sobel(gray,cv2.CV_64F,1,1,ksize=5)
plt.imshow(sobelxy,cmap='gray')
plt.title("Sobel XY axis")
plt.axis("off")
plt.show()
```
```
lap=cv2.Laplacian(gray,cv2.CV_64F)
plt.imshow(lap,cmap='gray')
plt.title("Laplacian Edge Detector")
plt.axis("off")
plt.show()
```
## Output:
### SOBEL EDGE DETECTOR
![image](https://github.com/user-attachments/assets/59796d27-2c90-494b-8580-a88a7bf8cfab)
![image](https://github.com/user-attachments/assets/cbc9d548-4a97-400c-b8e5-f443c7950d6b)
![image](https://github.com/user-attachments/assets/f63229dd-594c-4346-870a-a96753f4f6f5)
### LAPLACIAN EDGE DETECTOR
![image](https://github.com/user-attachments/assets/8546c7eb-7402-421b-a763-8e72eb4acf28)
### CANNY EDGE DETECTOR
![image](https://github.com/user-attachments/assets/0894e57f-8ee0-4929-9bb5-77e4d1de8d49)
## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
