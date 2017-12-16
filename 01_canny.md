```python
def proc(im):
    im = cv2.cvtColor(im, cv2.COLOR_BGR2GRAY)
    im = cv2.blur(im, (3, 3))
    im = cv2.Canny(im, 50, 100)
    im = cv2.cvtColor(im, cv2.COLOR_GRAY2BGR)

    return im
```

![](./images/00_src.png)

![](./images/01_canny.png)
