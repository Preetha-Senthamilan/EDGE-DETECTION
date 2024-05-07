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
DEVELOPED BY : PREETHA.S
REGISTER NO : 212222230110

```
## IMPORT PACKAGES AND LOAD IMAGES:

```
import cv2
import matplotlib.pyplot as plt

img=cv2.imread("preee.jpeg",0)
gray=cv2.cvtColor(img,cv2.COLOR_GRAY2RGB)
gray = cv2.GaussianBlur(gray,(3,3),0)

```
## SOBEL EDGE DETECTOR:

### SOBEL X:
```
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.imshow(sobelx,cmap='gray')
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
```

### SOBEL Y:
```
sobely = cv2.Sobel(gray,cv2.CV_64F,0,1,ksize=5)
plt.imshow(sobely,cmap='gray')
plt.title("Sobel Y axis")
plt.axis("off")
plt.show()
```

### SOBEL XY:
```
sobelxy = cv2.Sobel(gray,cv2.CV_64F,1,1,ksize=5)
plt.imshow(sobelxy,cmap='gray')
plt.title("Sobel XY axis")
plt.axis("off")
plt.show()

```

### LAPLACIAN EDGE DETECTOR:
```
lap=cv2.Laplacian(gray,cv2.CV_64F)
plt.imshow(lap,cmap='gray')
plt.title("Laplacian Edge Detector")
plt.axis("off")
plt.show()
```

### CANNY EDGE DETECTOR:
```
canny=cv2.Canny(gray,120,150)
plt.imshow(canny,cmap='gray')
plt.title("Canny Edge Detector")
plt.axis("off")
plt.show()

```

## Output:

![preee](https://github.com/Preetha-Senthamilan/EDGE-DETECTION/assets/119390282/6bcf9256-82f1-45ae-9186-f9d545a62595)


### SOBEL EDGE DETECTOR

### SOBEL X AXIS :

![image](https://github.com/Preetha-Senthamilan/EDGE-DETECTION/assets/119390282/1caccd95-7515-48cd-9dfe-6e3e38639ba3)

### SOBEL Y AXIS :

![image](https://github.com/Preetha-Senthamilan/EDGE-DETECTION/assets/119390282/a46c8b8d-a04b-4c0c-9423-71c4c39922bb)

### SOBEL XY AXIS :

![image](https://github.com/Preetha-Senthamilan/EDGE-DETECTION/assets/119390282/e9f20059-a640-44fa-8a11-123f51637f4b)


### LAPLACIAN EDGE DETECTOR

![image](https://github.com/Preetha-Senthamilan/EDGE-DETECTION/assets/119390282/c2d264d0-70c1-4d5d-ad48-b697f1bf8f67)



### CANNY EDGE DETECTOR

![image](https://github.com/Preetha-Senthamilan/EDGE-DETECTION/assets/119390282/6a392724-ba6a-4a71-b0fe-4792544f2a97)


## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
