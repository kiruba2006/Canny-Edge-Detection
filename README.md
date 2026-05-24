# WORKSHOP– 3  
# CANNY EDGE DETECTION

# Aim

To detect the edges of an image using Canny Edge Detection technique with Python and OpenCV.

---

# Software Required

- Anaconda – Python 3.7  
- OpenCV  
- Matplotlib  

---

# Algorithm

### Step 1:
Load the necessary packages.

### Step 2:
Read the input image in grayscale mode.

### Step 3:
Apply Gaussian Blur to reduce noise in the image.

### Step 4:
Apply Canny Edge Detection algorithm to detect edges.

### Step 5:
Display the original image and detected edge image.

---

# Program

### Developed By : Kiruba RC  
### Register Number : 212224230125

```python
import cv2
import matplotlib.pyplot as plt

# Read image in grayscale
img = cv2.imread('passport_photo.jpg', cv2.IMREAD_GRAYSCALE)

# Apply Gaussian Blur
blurred = cv2.GaussianBlur(img, (5,5), 0)

# Apply Canny Edge Detection
edges = cv2.Canny(blurred, 50, 150)

# Display images
plt.figure(figsize=(10,5))

plt.subplot(121)
plt.imshow(img, cmap='gray')
plt.title('Original Image')
plt.axis('off')

plt.subplot(122)
plt.imshow(edges, cmap='gray')
plt.title('Detected Edges')
plt.axis('off')

plt.show()
```

---

# Output

### Original Image

<img width="466" height="532" alt="image" src="https://github.com/user-attachments/assets/80ce3542-672a-4242-a23a-941aec89b840" />

### Detected Edges

<img width="452" height="538" alt="image" src="https://github.com/user-attachments/assets/665a7226-2c44-4498-870c-e1fc2b7e7f07" />


---

# Result

Thus the edges of the image are successfully detected using Canny Edge Detection technique with Python and OpenCV.
