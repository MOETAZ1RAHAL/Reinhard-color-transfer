# Reinhard Color Transfer

This project implements **Reinhard's color transfer algorithm** in Python using OpenCV.  
It allows you to **transfer the color palette** of a template image to an input image while preserving the structure of the original image. This is useful for color grading, image harmonization, and style transfer applications.

---

## How It Works

1. Convert input and template images to **Lab color space** (or log-LMS variant).  
2. Compute **per-channel mean and standard deviation** of both images.  
3. Adjust input image pixels to match the template’s mean and standard deviation.  
4. Convert the modified image back to **BGR** for display or saving.  

This simple statistical method produces visually pleasing color adjustments without complex neural networks.

---
## Original Paper

This work is based on the original research:

**Reinhard, E., Ashikhmin, M., Gooch, B., & Shirley, P. (2001). _Color Transfer between Images_.**  
PDF link: [https://www.cs.tau.ac.il/~turkel/imagepapers/ColorTransfer.pdf](https://www.cs.tau.ac.il/~turkel/imagepapers/ColorTransfer.pdf)

> Please cite this paper if you use this implementation in your research or projects.

---
