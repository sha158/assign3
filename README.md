# assign3
import numpy as np
import cv2
b = np.zeros([400,400],dtype='uint8')
n=50
j=n
while(j<=400) :
    i=n
    while(i<=400) :
        b[j-n:j,i-n:i] = 255
        b[j:j+n,i:i+n] = 255
        i=i+n*22
    j=j+n*2
cv2.imshow('checker board 8*8',b)
cv2.waitkey(0)
cv2.destroyAllWindows()
