```python
def proc(im):
    im = cv2.blur(im, (3, 3))
    im = cv2.adaptiveThreshold(im, 255, cv2.ADAPTIVE_THRESH_MEAN_C, cv2.THRESH_BINARY_INV, 11, 2)

    return im
```

![](./images/00_src.png)

![](./images/02_ada_thresh.png)
