# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
<br>

### Step2:
<br>

### Step3:
<br>

### Step4:
<br>

### Step5:
<br>

## Program:
```python
# Developed By:GANAPATHI VENKATESH
# Register Number:212220230018

# (i) bgr and rgb to hsv and gray

import cv2

img = cv2.imread('car.jpg')

#resizing the image to required size 
img= cv2.resize(img, (270,190))
cv2.imshow('INITIAL IMAGE',img)

#converting bgr image 2 hsv and grey
hsv_bgr = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsv_bgr)


gray_bgr = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',gray_bgr)


#converting bgr to rgb format 
bgr_rgb = cv2.cvtColor(img,cv2.COLOR_BGR2RGB)
cv2.imshow('BGR 2 RGB',bgr_rgb)
#rgb to hsv and grey
rgb_hsv = cv2.cvtColor(bgr_rgb,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2GRAY',rgb_hsv)

rgb_grey = cv2.cvtColor(bgr_rgb,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB 2 GREY',rgb_grey)
cv2.waitKey(0)

cv2.destroyAllWindows()

# (ii)Convert HSV to RGB and BGR

img = cv2.imread("car.jpg")

#resizing the image to required size 
img1= cv2.resize(img, (270,190))


#converting  bgr to hsv so it can be converted into rgb and bgr
hsv = cv2.cvtColor(img1 , cv2.COLOR_BGR2HSV)
cv2.imshow("INITIAL_HSV ", hsv)

#HSV TO RGB FORMAT
hsv_rgb = cv2.cvtColor(hsv, cv2.COLOR_HSV2RGB)
cv2.imshow("HSV2RGB", hsv_rgb)

#HSV TO BGR FORMAT
hsv_bgr = cv2.cvtColor(hsv, cv2.COLOR_HSV2BGR)
cv2.imshow("HSV_BGR", hsv_bgr)

cv2.waitKey(0)
cv2.destroyAllWindows()

# (iii)convert RGB and BGR to YCrCb

import cv2
 
img = cv2.imread("car.jpg")
img1= cv2.resize(img, (270,190))
cv2.imshow("BGR_COLOR ", img1)


#bgr to ycrcb

img_ycrcb = cv2.cvtColor(img1 , cv2.COLOR_BGR2YCrCb)
cv2.imshow("BGR_YCRCB ", img_ycrcb)


#converting  rgb to bgr so it can be converted into YCrCb

img_bgr = cv2.cvtColor(img1, cv2.COLOR_BGR2RGB)
cv2.imshow("RGB COLOR", img_bgr)

#rgb 2 ycrcb
img_bgr_y = cv2.cvtColor(img_bgr, cv2.COLOR_BGR2YCrCb)
cv2.imshow("RGB2YCrCb", img_bgr_y)

cv2.waitKey(0)
cv2.destroyAllWindows()

# (iv) Split and Merge RGB Image
img = cv2.imread("car.jpg")

#resizing the image to required size 
img1= cv2.resize(img, (270,190))

cv2

b,g,r = cv2.split(img1)

cv2.imshow("RED MODEL", r)
cv2.imshow("GREEN MODEL", g)
cv2.imshow("BLUE MODEL ", b)



#Merge:
merger = cv2.merge([b,g,r])
cv2.imshow("MERGED IMAGE", merger )


cv2.waitKey(0)

cv2.destroyAllWindows()


# (v)Split and merge HSV Image

img = cv2.imread("car.jpg")

#resizing the image to required size 
img1= cv2.resize(img, (270,190))


#converting  bgr to hsv so it can be converted into rgb and bgr
hsv = cv2.cvtColor(img1 , cv2.COLOR_BGR2HSV)
cv2.imshow("INITIAL_HSV ", hsv)


h,s,v = cv2.split(hsv)

cv2.imshow("RED MODEL", h)
cv2.imshow("GREEN MODEL", s)
cv2.imshow("BLUE MODEL ", v)



#Merge:
merger = cv2.merge([h,s,v])
cv2.imshow("MERGED IMAGE", merger )


cv2.waitKey(0)

cv2.destroyAllWindows()







```
## Output:
i) BGR and RGB to HSV and GRAY
![image1](https://github.com/20004426-venkatesh/Color-Conversion/blob/main/exp%203.1.jpg)


ii) HSV to RGB and BGR

![image1](https://github.com/20004426-venkatesh/Color-Conversion/blob/main/exp%203.2.jpg)
iii) RGB and BGR to YCrCb

![image1](https://github.com/20004426-venkatesh/Color-Conversion/blob/main/exp%203.3.jpg)
iv) Split and merge RGB Image

![image1](https://github.com/20004426-venkatesh/Color-Conversion/blob/main/exp%203.4.jpg)
v) Split and merge HSV Image
![image1](https://github.com/20004426-venkatesh/Color-Conversion/blob/main/exp%203.5.jpg)


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
