# Image-Processing-Stripe-Width
This is a jupyter notbook file for measuring stripe width of monolayer systems and binary images.

Here is an example image of a thresholded monolayer of DPPC, hexadeconal, and cholesterol. 
![example](https://github.com/b-solberg/Image-Processing-Stripe-Width/blob/main/Image12826-thresh.png)

In this image, we want to measure the width of the white stripes, after doing so we will output a histogram and a .csv files to save measurements.

---

This project uses basic image processing techniques such as the 'opening' method and skeletonization. 

The opening method erodes white pixels then dilations the left over pixels and specifically in this case uses a disk structuring kernel. THe skeletonization method is used to count all the width measurements. 
