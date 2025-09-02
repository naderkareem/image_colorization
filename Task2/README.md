Artistic Style Transfer with Image Colorization

Overview

This project implements Task 2: an application that colorizes grayscale images and applies artistic style transfer to the colorized outputs, using a U-Net model for colorization and VGG19 for style transfer. A tkinter-based graphical user interface (GUI) allows users to upload grayscale images, select from predefined artistic styles (Van Gogh, Monet, Ukiyo-e), and save the stylized, colorized results. The application processes images at 256x256 resolution for improved visual quality, leveraging a pretrained U-Net model hosted on Google Drive due to GitHub’s 100MB file size limit: Model Files.

Features

Colorization: Uses a pretrained U-Net model to convert grayscale images to RGB, optimized for accuracy and smooth outputs.
Style Transfer: Applies artistic styles (Van Gogh, Monet, Ukiyo-e) using VGG19-based content and style losses, with 200 optimization steps for enhanced stylization.
GUI: tkinter interface for uploading grayscale images, selecting styles, and saving outputs as PNG files.
Resolution: Processes images at 1024x1024 for better detail, with U-Net outputs upsampled from 32x32 using bilinear interpolation.
Error Handling: Includes robust model loading with fallback to weights and error messages for missing style images or models.


Download Pretrained Model:
Download model_mse.pth and model_mse_weights.pth from Google Drive.



Create a Virtual Environment:python -m venv env
env\Scripts\activate  # Windows


Install Dependencies:pip install -r requirements.txt


Ensure CUDA (Optional):
The script uses CPU if CUDA is unavailable. For GPU support, ensure CUDA is compatible with PyTorch 2.0.1.



Usage

Run the Application:python colorization_style_transfer.ipynb


GUI Instructions:
Select Style: Choose Van Gogh, Monet, or Ukiyo-e from the dropdown menu.
Upload Image: Click “Upload Image” to select a grayscale image (.jpg, .jpeg, .png).
Process: Click “Colorize & Apply Style” to generate and display the stylized, colorized image (256x256).
Save: Click “Save Output” to save the result as a PNG file.


Outputs:
Image: Stylized, colorized image displayed via the GUI and saved (e.g., output.png).
Console: Messages indicating model loading or errors (e.g., missing model or style images).



