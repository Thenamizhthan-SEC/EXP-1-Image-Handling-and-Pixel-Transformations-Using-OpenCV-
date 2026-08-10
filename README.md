# EXP-1-Image-Handling-and-Pixel-Transformations-Using-OpenCV-
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
- **Name:** Thenamizhthan V 
- **Register Number:** 212225240175

  ### Ex. No. 01

#### 1. Read the image ('then.jpg') using OpenCV imread() as a grayscale image.
```
python
plt.imshow(image_gray, cmap='gray')
plt.title("Grayscale Image")
plt.axis("off")

```

#### 2.Draw a line from the top-left to the bottom-right of the image.
```
# Load the image
image = cv2.imread('then.jpg')
# Convert BGR (OpenCV's default) to RGB (Matplotlib's expected color order)
img_rgb = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
img_rgb.shape
(4000, 3000, 3
line_img = cv2.line(img_rgb, (0, 0), (768, 600), (255, 0, 0), 2) # cv2.line(image, start_point, end_point, color, thickness)
```

#### Draw a circle at the center of the image.
```
python
plt.imshow(circle_img, cmap='viridis')  
plt.title("Image with Circle")
plt.axis('off')  
plt.show()

```

#### Draw a rectangle around  the whole image
```
python
plt.imshow(rectangle_img, cmap='viridis')  
plt.title("Image with Rectangle")
plt.axis('off')  
plt.show()
```

#### 5. Add the text "OpenCV Drawing" at the top-left corner of the image.
```
python
text_img = cv2.putText(img_rgb, "Thenamizhthan", (10, 1), cv2.FONT_HERSHEY_SIMPLEX, 1, (255, 800, 255), 10)  ## cv2.putText(image, text, position, font, font_scale, color, thickness)
```

#### 6. Convert the image from RGB to HSV and display it.
```
python
# HSV Image
plt.imshow(image_hsv)
plt.title("HSV Image")
plt.axis("off")
```

#### 7. Convert the image from RGB to GRAY and display it.
```
python
plt.imshow(image_gray, cmap='gray')
plt.title("Grayscale Image")
plt.axis("off")
```

#### Convert the image from RGB to YCrCb and display it.
```
python
# YCrCb Image
plt.imshow(image_ycrcb)
plt.title("YCrCb Image")
plt.axis("off")
```

#### 9. Convert the HSV image back to RGB and display it.
```
python
plt.imshow(image_hsv_to_rgb)
plt.title("HSV to RGB Image")
plt.axis("off")
```

#### Resize the original image to half its size and display it.
```
python
plt.imshow(resized_image_rgb)
plt.title("Resized Image (Half Size)")
plt.axis("off")
plt.show()
```

#### Crop a region of interest (ROI) from the image (e.g., a 100x100 pixel area starting at (50, 50)) and display it.:
```
python
# Display the cropped region (ROI)
plt.imshow(roi_rgb)
plt.title("Cropped Region of Interest (ROI)")
plt.axis("off")
plt.show()
```

#### 12.Flip the original image horizontally and display it.
```
python
rect_color = magenta
# Horizontal flip
plt.imshow(flipped_horizontally_rgb)
plt.title("Flipped Horizontally")
plt.axis("off")
```

#### Flip the original image vertically and display it
```
python
# Vertical flip
plt.imshow(flipped_vertically_rgb)
plt.title("Flipped Vertically")
plt.axis("off")
```


## Output:
- **i)** Read and Display an Image.  
- **ii)** Adjust Image Brightness.  
- **iii)** Modify Image Contrast.  
- **iv)** Generate Third Image Using Bitwise Operations.

## Result:
Thus, the images were read, displayed, brightness and contrast adjustments were made, and bitwise operations were performed successfully using the Python program.
