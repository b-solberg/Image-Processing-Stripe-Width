# Image-Processing-Stripe-Width
This is a jupyter notbook file for measuring stripe width of monolayer systems and binary images.

Here is an example image of a thresholded monolayer of DPPC, hexadeconal, and cholesterol. 

![example](https://github.com/b-solberg/Image-Processing-Stripe-Width/blob/main/Image12826-thresh.png)

In this image, we want to measure the width of the white stripes, after doing so we will output a histogram and a .csv files to save measurements.

---

### Getting Started

Python and Jupyter notebooks are required. Versions of image processing libraries are included in the .ipynb file. 

Once running the notebook, the only user inputs are the file path to the image, a ```junction_cutoff``` variable to remove junctions between stripes/branches, and a ```pixel_to_micron``` to convert pixels to microns (or other distance units). ```junction_cutoff``` is used because the junctions between stripes/branches are wider than the actual stripe width. Adjust until the first image to pop up has 'holes' cut out and no other areas of the stripes are removed (as small as possible in otherwords). 

---
### Image Processing Basics

This project uses basic image processing techniques such as the 'opening' method and skeletonization. 

The opening method erodes white pixels then dilations the left over pixels and specifically in this case uses a disk structuring kernel. The skeletonization method is used to count all the width measurements. 

---
