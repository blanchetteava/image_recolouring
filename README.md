# image_recolouring
Recolouring images in R by mapping normalized grayscale values onto a custom colour palette.


Overview

This project demonstrates how to transform an image by converting it into normalized grayscale values and then recolouring it with a custom colour palette using R. The workflow crops and resizes the input image, extracts pixel brightness values, normalizes them to a 0–1 scale, and maps them onto a user-defined palette to produce a stylized rendering.
Repository Contents
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
