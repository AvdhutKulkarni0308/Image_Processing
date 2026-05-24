# Noise Models and Image Restoration using Filters

This project demonstrates various **Noise Models** and **Image Restoration Techniques** using Python and OpenCV.
The experiment focuses on restoring degraded images using:

* Arithmetic Mean Filter
* Midpoint Filter
* Alpha-Trimmed Mean Filter

---

# 📌 Aim

To study different noise models and restore a degraded image using spatial domain filters.

---

# 🛠️ Software Requirements

* Python 3.x
* OpenCV
* NumPy
* Matplotlib
* Google Colab / Jupyter Notebook

---

# 📚 Theory

## Noise Models

Noise degrades image quality during acquisition or transmission.

### Types of Noise

### 1. Gaussian Noise

* Caused by sensor and electronic circuit disturbances.
* Random intensity variations.

### 2. Salt and Pepper Noise

* Appears as random black and white pixels.
* Usually caused by transmission errors.

### 3. Uniform Noise

* Noise values are uniformly distributed over a range.

---

# 🧹 Image Restoration Filters

## 1. Arithmetic Mean Filter

The arithmetic mean filter replaces each pixel with the average value of neighboring pixels.

### Formula

\hat{f}(x,y)=\frac{1}{mn}\sum_{(s,t)\in S_{xy}} g(s,t)

### Advantages

* Reduces Gaussian noise
* Simple implementation

### Disadvantages

* Blurs image edges

---

## 2. Midpoint Filter

The midpoint filter computes the average of maximum and minimum pixel values.

### Formula

\hat{f}(x,y)=\frac{1}{2}[\max(g(s,t))+\min(g(s,t))]

### Advantages

* Effective for uniform noise

---

## 3. Alpha-Trimmed Mean Filter

Removes extreme pixel values before computing the mean.

### Formula

\hat{f}(x,y)=\frac{1}{mn-d}\sum g_r(s,t)

Where:

* `d` = number of removed pixels

### Advantages

* Works well for both Gaussian and impulse noise

---

# 🧪 Filters Implemented

| Filter                    | Purpose                                  |
| ------------------------- | ---------------------------------------- |
| Arithmetic Mean Filter    | Smooths image and reduces Gaussian noise |
| Midpoint Filter           | Reduces uniform noise                    |
| Alpha-Trimmed Mean Filter | Removes Gaussian + impulse noise         |

---


# 💻 Technologies Used

* Python
* OpenCV
* NumPy
* Matplotlib

---


# ✅ Result

Thus, various noise models were studied and the degraded image was successfully restored using Arithmetic Mean, Midpoint, and Alpha-Trimmed Mean filters.
