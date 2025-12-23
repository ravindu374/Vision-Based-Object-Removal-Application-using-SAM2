# Vision-Based Object Removal Application using SAM2

## Overview

This project implements a vision-based user application for interactive object removal from images. It extends the **SAM2 segmentation model** into a practical tool that allows users to select and remove unwanted objects. The removed regions are reconstructed using the **Telea inpainting algorithm**, producing visually consistent results.

The project focuses on applying segmentation and classical image restoration techniques to build a usable computer vision application, rather than training new models.

---

## Features

- Interactive object selection using SAM2  
- Precise segmentation mask generation  
- Object removal using Telea inpainting  
- No model retraining required  
- Image-level processing  

---

## System Workflow

1. User provides an input image  
2. Object is selected using guided prompts  
3. SAM2 generates a segmentation mask  
4. Mask is refined for clean boundaries  
5. Telea inpainting fills the removed region  
6. Final image is produced  

---

## Technologies Used

- Python  
- SAM2 segmentation model  
- OpenCV  
- Telea inpainting  
- NumPy  
- Jupyter Notebook  

---

## Why Telea Inpainting?

The Telea inpainting algorithm is fast, lightweight, and well suited for interactive object removal tasks. It provides reliable visual results for small to medium objects and allows quick feedback without the overhead of deep learning–based inpainting models.

---



---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git

2. Install dependencies:
   ```bash
    pip install -r requirements.txt

3. Open the notebook:
   ```bash
    jupyter notebook Delete_Object.ipynb

4. Follow the instructions in the notebook to remove objects.
