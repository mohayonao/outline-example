```python
def proc(im):
    im = cv2.blur(im, (3, 3))
    im = cv2.Canny(im, 50, 100)

    return im
```

![](./images/00_src.png)

![](./images/01_canny.png)
