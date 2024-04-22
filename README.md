# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages


### Step2:
Read the image

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

### Step6:
Display all the output images

 
## Program:
```
Developed By: SIVABALAN S
Register NO: 212221240100
```
``` Python
# Import the necessary packages
import cv2
import numpy as np

# Create the Text using cv2.putText
img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'IMMACUALTE', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)

# Create the structuring element
struct_ele = np.ones((9, 9), np.uint8)

# Use Opening operation
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)

# Use Closing Operation
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)

# Close all windows
cv2.destroyAllWindows()
```
## Output:

### Display the input Image
![Screenshot 2024-04-22 232629](https://github.com/sivabalan28/OPENING--AND-CLOSING/assets/113497347/ee78e90c-fd7e-4275-8f57-f1a6b3be19ca)


### Display the result of Opening
![Screenshot 2024-04-22 232640](https://github.com/sivabalan28/OPENING--AND-CLOSING/assets/113497347/75594a10-cf45-45d0-9992-e55f40d3657d)


### Display the result of Closing
![Screenshot 2024-04-22 232650](https://github.com/sivabalan28/OPENING--AND-CLOSING/assets/113497347/bbb8857b-5b98-40f2-a9a8-9bb0c4347d17)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
