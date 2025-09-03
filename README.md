# image_recolouring
Recolouring images in R by mapping normalized grayscale values onto a custom colour palette.

# Overview

This Rmd contains a base for simple (and fun) image processing in R. This script takes an input photo, crops and resizes it, then converts it to greyscale so that every pixel is represented by a brightness value. These values, which originally range from 0 (black) to 255 (white), are normalised—rescaled to fit between 0 and 1 for easier handling. The pixel grid is then rebuilt as a data frame, and each pixel’s brightness is mapped onto a custom color palette (instead of plain gray), effectively “repainting” the image with new tones. For complete colour freedom, please refer to: https://sites.stat.columbia.edu/tzheng/files/Rcolor.pdf

For reproducibility, users are encouraged to replace the file paths and image files with their own.

Repository Contents:
input/ – Example input images
output/ – Generated output images
image_render.Rmd – R Markdown file containing the full workflow
image_render.html – HTML export of the R Markdown notebook

Method
Preprocessing – Load the image, crop to a centered square, and resize.
Grayscale Conversion – Convert pixels to brightness values (0 = black, 255 = white).
Normalization – Rescale grayscale values to a standard 0–1 range.
Recolouring – Map normalized values onto a custom colour palette.
Rendering – Plot the recoloured grid of pixels using ggplot2 and save as PNG.
