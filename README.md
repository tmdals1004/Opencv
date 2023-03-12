# Opencv 컬러,흑백
```python
import matplotlib.pyplot as plt
import cv2
#컬러
imgBGR = cv2.imread('cat.bmp') #실행중인 파이썬의 경로와 같은 경로에 사진있어야함
imgRGB = cv2.cvtColor(imgBGR,cv2.COLOR_BGR2RGB) #opencv가 읽는 컬러로 받아옴

plt.axis('off')
plt.imshow(imgRGB)
plt.show()
#흑백
imgGray = cv2.imread('cat.bmp',cv2.IMREAD_GRAYSCALE)

plt.axis('off')
plt.imshow(imgGray,cmap='gray')
plt.show()
```
