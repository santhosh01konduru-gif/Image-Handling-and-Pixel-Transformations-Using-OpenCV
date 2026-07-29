# Image-Handling-and-Pixel-Transformations-Using-OpenCV 

## AIM:
Write a Python program using OpenCV that performs the following tasks:

1) Read and Display an Image.  
2) Adjust the brightness of an image.  
3) Modify the image contrast.  
4) Generate a third image using bitwise operations.

## Software Required:
- Anaconda - Python 3.7
- Jupyter Notebook (for interactive development and execution)

## Algorithm:
### Step 1:
Load an image from your local directory and display it.

### Step 2:
Create a matrix of ones (with data type float64) to adjust brightness.

### Step 3:
Create brighter and darker images by adding and subtracting the matrix from the original image.  
Display the original, brighter, and darker images.

### Step 4:
Modify the image contrast by creating two higher contrast images using scaling factors of 1.1 and 1.2 (without overflow fix).  
Display the original, lower contrast, and higher contrast images.

### Step 5:
Split the image (boy.jpg) into B, G, R components and display the channels

## Program Developed By:
- **Name:** konduru santhosh
- **Register Number:** 212225240074

  ### Ex. No. 01

#### 1. Read the image using OpenCV 
```python
import cv2
import matplotlib.pyplot as plt
# Read the image using OpenCV
img = cv2.imread('BIRD.jpg', cv2.IMREAD_COLOR)
```

#### 2. Convert BGR (OpenCV's default) to RGB (Matplotlib's expected color order)
```python
# Convert BGR (OpenCV's default) to RGB (Matplotlib's expected color order)
img_rgb = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
```

#### 3. Display the image using matplotlib imshow().
```python
# Display the image using Matplotlib
plt.imshow(img_rgb, cmap='viridis')  # You can change 'viridis' to another cmap or use None for RGB images
plt.title("Original Image")
plt.axis('on')  # Removes axis ticks and labels
plt.show()
```

#### 4. load the image
```python
# Load the image
image = cv2.imread('BIRD.jpg')
```

#### 5. Read the saved image above as a color image using cv2.cvtColor().
```python
# Convert BGR (OpenCV's default) to RGB (Matplotlib's expected color order)
img_rgb = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
```

#### 6. Draw a line from top left to right bottom
```python
img_rgb.shape
line_img = cv2.line(img_rgb, (0, 0), (8192,4096), (255,0, 0), 15) # cv2.line(image, start_point, end_point, color, thickness)
```

#### 7. load the image
```python
image = cv2.imread('BIRD.jpg')
```

#### 8. Convert BGR (OpenCV's default) to RGB (Matplotlib's expected color order)
```python
# Convert BGR (OpenCV's default) to RGB (Matplotlib's expected color order)
img_rgb = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
```

#### 9. Draw acircle shape in the image
```python
img_rgb.shape
circle_img = cv2.circle(img_rgb,(4096,2048),750,(255,0,0),15) # cv2.circle(image, center, radius, color, thickness)
plt.imshow(circle_img, cmap='viridis')  
plt.title("Image with Circle")
plt.axis('on')  
plt.show()
```

#### 10. Read in the image ('Apollo-11-launch.jpg').
```python
# YOUR CODE HERE
```

#### 11. Add the following text to the dark area at the bottom of the image (centered on the image):
```python
text = 'Apollo 11 Saturn V Launch, July 16, 1969'
font_face = cv2.FONT_HERSHEY_PLAIN
# YOUR CODE HERE: use putText()
```

#### 12. Draw a magenta rectangle that encompasses the launch tower and the rocket.
```python
rect_color = magenta
# YOUR CODE HERE
```

#### 13. Display the final annotated image.
```python
# YOUR CODE HERE
```

#### 14. Read the image ('Boy.jpg').
```python
# YOUR CODE HERE
```

#### 15. Adjust the brightness of the image.
```python
# Create a matrix of ones (with data type float64)
# matrix_ones = 
# YOUR CODE HERE
```

#### 16. Create brighter and darker images.
```python
img_brighter = cv2.add(img, matrix)
img_darker = cv2.subtract(img, matrix)
# YOUR CODE HERE
```

#### 17. Display the images (Original Image, Darker Image, Brighter Image).
```python
# YOUR CODE HERE
```

#### 18. Modify the image contrast.
```python
# Create two higher contrast images using the 'scale' option with factors of 1.1 and 1.2 (without overflow fix)
matrix1 = 
matrix2 = 
# img_higher1 = 
# img_higher2 = 
# YOUR CODE HERE
```

#### 19. Display the images (Original, Lower Contrast, Higher Contrast).
```python
# YOUR CODE HERE
```

#### 20. Split the image (boy.jpg) into the B,G,R components & Display the channels.
```python
# YOUR CODE HERE
```

#### 21. Merged the R, G, B , displays along with the original image
```python
# YOUR CODE HERE
```

#### 22. Split the image into the H, S, V components & Display the channels.
```python
# YOUR CODE HERE
```
#### 23. Merged the H, S, V, displays along with original image.
```python
# YOUR CODE HERE
```

## Output:
- **i)** Read and Display an Image.  
- **ii)** Adjust Image Brightness.  
- **iii)** Modify Image Contrast.  
- **iv)** Generate Third Image Using Bitwise Operations.
- <img width="263" height="434" alt="image" src="https://github.com/user-attachments/assets/db54f04b-dd2a-43ae-b1be-299b9da404ff" />
<img width="263" height="434" alt="image" src="https://github.com/user-attachments/assets/2e25b220-1ea8-4650-a764-d4eb38aa64e6" />
<img width="263" height="434" alt="image" src="https://github.com/user-attachments/assets/8fe8cd67-e610-41e3-bd8d-3e41ac9e6de2" />
<img width="263" height="434" alt="image" src="https://github.com/user-attachments/assets/bb9f6319-6a4b-4fe7-9708-5af0926ae768" />
<img width="226" height="410" alt="image" src="https://github.com/user-attachments/assets/710419ff-ba96-4064-ae9c-ff5e66dc9869" />
<img width="263" height="434" alt="image" src="https://github.com/user-attachments/assets/abbdb755-1839-40ef-a1ff-12596e2b826f" />
<img width="226" height="410" alt="image" src="https://github.com/user-attachments/assets/ac3ccce8-1428-4d1f-a752-4b7358a8de5b" />
<img width="226" height="410" alt="image" src="https://github.com/user-attachments/assets/23be0516-3438-4bf3-960e-923ce3043cf3" />
<img width="226" height="410" alt="image" src="https://github.com/user-attachments/assets/c8589060-d599-49e0-8540-9e7158dcc8cb" />
<img width="226" height="410" alt="image" src="https://github.com/user-attachments/assets/36a82b39-5172-4375-a9e9-b415a45c4855" />










## Result:
Thus, the images were read, displayed, brightness and contrast adjustments were made, and bitwise operations were performed successfully using the Python program.

