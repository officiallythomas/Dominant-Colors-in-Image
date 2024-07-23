# Dominant-Colors-in-Image

Computer vision techniques and clustering algorithms to analyze and visually represent the dominant colors present in the input image, providing insights into its color composition.

This task of identifying the predominant colors in the input image involves analyzing the pixel data of the image to determine which colors appear most frequently or prominently. This process typically includes the following steps:

This script performs color analysis on an image using the K-means clustering algorithm to identify dominant colors. 

1. **Loading and Resizing Image:**
   - Loaded the image using OpenCV (`cv2.imread`). It creates a copy of the original image.
   - The image is resized to a height of 200 pixels using `imutils.resize`. The resized image shape is printed to confirm the new dimensions.

2. **Flattening Image:**
   - The image is flattened into a 2D array (`flat_img`) where each row represents a pixel and its RGB values. This is achieved using NumPy's `reshape` function.

3. **Applying K-means Clustering:**
   - K-means clustering is applied to flattened image to group similar colors into  clusters.
   - The cluster centers  represent the dominant colors in the image, converted to a type for RGB values.

4. **Calculating Color Percentages:**
   - Percentages of each dominant color are calculated based on the number of pixels assigned to each cluster.

5. **Visualizing Dominant Colors:**
   - Matplotlib is used to visualize the dominant colors in two ways:
     - Subplots displaying each dominant color as a block with its percentage.
     - A bar chart representing the proportion of each color across the image.
  ![](https://github.com/officiallythomas/Dominant-Colors-in-Image/blob/main/Dominant%20color%20percent.jpg)

6. **Enhancing Image Visualization:**
   - The original image is resized for better display, and a translucent rectangle is overlaid on the top half to enhance readability of text.

7. **Adding Text and Dominant Colors to Image:**
   - Text indicating "Most Dominant Colors in the Image" is added to  the final enhanced image.
   - The top 5 dominant colors are displayed as color blocks with corresponding rank numbers on final image.

8. **Displaying and Saving Results:**
   - Matplotlib and OpenCV are used to display the final image with dominant colors and text.
   
 ![](https://github.com/officiallythomas/Dominant-Colors-in-Image/blob/main/color%20proportion.jpg)


