Image Colorization Project
This repository contains a Python script (conditional_colorization.py) for conditionally colorizing grayscale images using a pretrained U-Net model. Users can specify colors for selected regions (e.g., blue for sky, green for grass) via a tkinter GUI, with seamless blending to ensure natural-looking outputs at 512x512 resolution.
Overview

Task 3: Implements conditional image colorization with a GUI for region selection and color picking.
Model: Uses a pretrained U-Net (model_mse.pth) trained on CIFAR-100, upsampled to 512x512 with bicubic interpolation.
Features: Upload grayscale images, draw bounding boxes, choose colors, and save colorized outputs.

Prerequisites

Python: 3.8 or higher
OS: Windows (compatible with CUDA if available)
Dependencies: Install via requirements.txt:




Set Up Virtual Environment:
python -m venv env
env\Scripts\activate


Install Dependencies:
pip install -r requirements.txt


Download Pretrained Model:

Download model_mse.pth and model_mse_weights.pth from Google Drive.



GUI Operations:

Upload Image: Click "Upload Image" to select a grayscale image (.jpg, .jpeg, .png).
Choose Color: Click "Choose Color" to pick an RGB color (e.g., blue: (0, 0, 255), green: (0, 255, 0)).
Draw Regions: Click and drag on the canvas to draw a bounding box over a region; repeat for multiple regions.
Colorize: Click "Colorize with Conditions" to generate and display the 512x512 colorized image.
Save: Click "Save Output" to save the result as a .png.


Expected Output:

A 512x512 colorized image with user-specified colors blended naturally into the U-Net’s output.



