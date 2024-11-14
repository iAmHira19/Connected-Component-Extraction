
# Connected Component Estimation in Python

This repository contains a Python script for estimating connected components in a grayscale image. The script performs several processing steps, including thresholding, inversion, connected component analysis, and visualizing each component with a unique color. It’s designed to help users understand and present connected component analysis in computer vision.

## Table of Contents
- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Explanation of Each Step](#explanation-of-each-step)
- [Example Output](#example-output)

## Overview

This script takes a grayscale image as input and:
1. Converts it to a binary image.
2. Performs connected component analysis to identify distinct components.
3. Assigns a unique color to each component for visualization.

The code is structured for ease of understanding and can be used for educational purposes or demonstrations.

## Prerequisites

To run this script, you’ll need:
- **Python 3.x**
- **OpenCV**: `pip install opencv-python`
- **NumPy**: `pip install numpy`
- **Matplotlib**: `pip install matplotlib`

**Note:** This script is designed to work in a Jupyter Notebook or Google Colab environment for ease of image upload and display.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/connected-component-estimation.git
   ```
2. Navigate to the project directory:
   ```bash
   cd connected-component-estimation
   ```

## Usage

1. Open the script in Google Colab or any Jupyter Notebook environment.
2. **Upload an Image**: The script will prompt you to upload a grayscale image for analysis.
3. Run the code to display the original image, binary image, and the connected components image with each region colored uniquely.

## Explanation of Each Step

1. **Image Input**: Prompts the user to upload an image file.
2. **Image Loading**: Reads the image in grayscale format, converting it to a NumPy array compatible with OpenCV functions.
3. **Binary Thresholding**: Converts the grayscale image to a binary image by applying a threshold. Pixels below 128 become black (0), and pixels above 128 become white (255).
4. **Inversion**: Inverts the binary image so the background is black, and the foreground is white, preparing it for connected component analysis.
5. **Connected Components Analysis**: Analyzes the binary image to label connected regions, and assigns each a unique label.
6. **Component Counting**: Displays the number of connected components, excluding the background.
7. **Color Assignment**: Each labeled component is assigned a random color for visualization, differentiating each region.
8. **Image Display Function**: Uses Matplotlib to display images inline with titles.
9. **Display Results**: Shows the original, binary, and connected components images for comparison.

## Example Output

After running the script, you will see three images:
- **Original Image**: The input grayscale image.
- **Binary Image**: The processed binary image.
- **Connected Components**: Each connected component displayed in a unique color for easy identification.




