# README.md — Experiment No. 5

# Edge Detection using Canny and Sobel Algorithms

## 📌 Aim

To detect the edges of a given input image using the following edge detection algorithms:

* Sobel Edge Detection
* Canny Edge Detection



# 📚 Theory

## Edge Detection

Edge detection identifies points in an image where intensity changes abruptly.
These points correspond to object boundaries and are important for:

* Image Analysis
* Image Segmentation
* Feature Extraction


---

# 1️⃣ Sobel Edge Detection

## Theory

Sobel operator uses first-order derivatives to calculate image gradients in horizontal and vertical directions.


## Sobel Kernels

### Horizontal Gradient (Gx)

```text id="0aj2c8"
| -1   0   1 |
| -2   0   2 |
| -1   0   1 |
```

### Vertical Gradient (Gy)

```text id="y9vkx0"
| -1  -2  -1 |
|  0   0   0 |
|  1   2   1 |
```

### Gradient Magnitude

```text id="w1u85x"
G = √(Gx² + Gy²)
```


---

## Gradient Magnitude

```text id="5a2k1r"
G = √(Gx² + Gy²)
```


##  Algorithm

1. Read grayscale image
2. Apply Sobel operator in horizontal and vertical directions
3. Compute gradient magnitude
4. Display edge detected image



# 2️⃣ Canny Edge Detection

## Theory

Canny edge detection is a multi-stage algorithm that produces thin and continuous edges.

### Steps Involved

* Gaussian Smoothing
* Gradient Calculation
* Non-Maximum Suppression
* Double Thresholding
* Edge Tracking using Hysteresis

Reference: 

---

##  Algorithm

1. Read grayscale image
2. Apply Gaussian Blur
3. Compute gradient magnitude and direction
4. Perform non-maximum suppression
5. Apply double thresholding
6. Track edges using hysteresis

---


# 💻 Technologies Used

* Python
* OpenCV
* NumPy
* Matplotlib

---

# ✅ Result

Thus, edges of the given input image were successfully detected using Sobel and Canny edge detection algorithms.

---