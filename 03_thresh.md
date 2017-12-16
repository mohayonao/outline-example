```python
def proc(im):
    im = cv2.cvtColor(im, cv2.COLOR_BGR2GRAY)
    im = cv2.blur(im, (3, 3))
    im = cv2.threshold(im, 128, 255, cv2.THRESH_BINARY)[1]

    return im
```

![](./images/00_src.png)

![](./images/03_thresh.png)
