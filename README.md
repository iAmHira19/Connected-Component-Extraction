# Connected-Component-Extraction

Image Input: The user is prompted to enter an image file path, allowing the program to work with any grayscale image.
Image Loading: Loads the image in grayscale, where each pixel intensity is a shade between black and white.
Binary Thresholding: Converts the grayscale image to a binary image (black and white) by setting a threshold value. Pixels below 128 become black, and those above 128 become white.
Inversion: Ensures that the foreground is white (255), and the background is black (0), preparing the image for connected component analysis.
Connected Components Analysis: Identifies connected regions in the binary image and assigns each a unique label. It also calculates the statistics and centroids for each component.
Component Counting: Displays the number of components, excluding the background.
Color Assignment: Each labeled component is displayed in a random color for visual differentiation.
Image Display Function: Uses matplotlib to show images inline with titles.
Display Results: Shows the original image, the binary (processed) version, and the connected component image with each region colored.
