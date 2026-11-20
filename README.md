### NAME: SURYA P <br>
### REG NO: 212224230280 <br> 
### Date: 20/11/2026

## EX. No. 9 : RECORD IMPLEMENTATION OF EROSION AND DILATION

## Aim:

To write a Python program using OpenCV to perform morphological operations such as Erosion and Dilation on an image.

The program performs the following operations:

- Image Erosion
- Image Dilation

## Software Used:

- Anaconda – Python 3.7
- Jupyter Notebook / VS Code
- OpenCV (cv2)
- NumPy
- Matplotlib

## Algorithm:

### Step 1:

Import the required libraries: OpenCV, NumPy, and Matplotlib.

### Step 2:

Create a blank image using NumPy.

### Step 3:

Insert text onto the image using OpenCV's text drawing function.

### Step 4:

Display the original image.

### Step 5:

Create a structuring element (kernel) of suitable size.

### Step 6: Image Erosion:

- Apply the erosion operation using the created kernel.
- Remove pixels from the boundaries of foreground objects.
- Display the eroded image.

### Step 7: Image Dilation:

- Apply the dilation operation using the same kernel.
- Add pixels to the boundaries of foreground objects.
- Display the dilated image.

### Step 8:

Compare the original, eroded, and dilated images.

## Program:

Developed By

**Name:** SURYA P

**Register No:** 212224230280

## Output:

### Original Image:
```
import cv2
import matplotlib.pyplot as plt
img = cv2.imread("image.png")
plt.imshow(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
plt.title("Original Image")
plt.axis("off")
plt.show()

```
<img width="515" height="531" alt="image" src="https://github.com/user-attachments/assets/cdb92db3-80aa-48fe-be19-39cbdabed1b9" />


### Erosion:
```
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
erosion = cv2.erode(img, kernel, iterations=1)
plt.imshow(erosion, cmap="gray")
plt.title("Image Erosion")
plt.axis("off")
plt.show()
```

<img width="541" height="537" alt="image" src="https://github.com/user-attachments/assets/3a856da9-5166-4858-bd42-55add16eef4d" />


### Dilation:
```
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
dilation = cv2.dilate(img, kernel, iterations=1)
plt.imshow(dilation, cmap="gray")
plt.title("Image Dilation")
plt.axis("off")
plt.show()
```
<img width="535" height="528" alt="image" src="https://github.com/user-attachments/assets/1784360c-4866-4abf-9a21-7016afefad4e" />


## Result:

Thus, the morphological operations **Erosion** and **Dilation** are successfully implemented using OpenCV.
