# Double
import cv2 as cv
import numpy as np
d = 400
img = np.ones((d,d,3),dtype='uint8')*255
font = cv.FONT_HERSHEY_SIMPLEX #字體名稱 : HERSHEY_SIMPLEX
cv.putText(img, 'OpenCV',(0,200),font,3,(0,255,0),15)
#描邊就是利用筆畫的粗細，可修改值:15
cv.putText(img, 'OpenCV',(0,200),font,3,(0,0,255),5)
cv.imshow('image', img)
cv.waitKey()
