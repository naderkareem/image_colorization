Task 4 – Dataset Augmentation for Image Colorization

This task implements a deep learning model for image colorization with a focus on improving performance using data augmentation techniques.
The model is trained on CIFAR-10 images and produces enhanced colorization results by leveraging transformations such as rotation, flipping, affine transformations, and brightness/contrast adjustments.

📝 Overview

Dataset: CIFAR-10 (automatically downloaded if missing).

Model: Encoder–Decoder CNN (ColorizationNet) with three convolutional encoder layers and a decoder.

Loss Function: Weighted combination of

Mean Squared Error (MSE) Loss

Perceptual Loss (from a pre-trained VGG16 network).

Key Features:

Grayscale-to-color image translation.

Robust training with data augmentation for better generalization.

Visualization of original, grayscale, and colorized outputs.

Saves trained models (.pth) and weights for reuse.

⚙️ Requirements

Python 3.8+

Recommended: GPU with CUDA (CPU is supported but slower).

Install dependencies:

pip install torch torchvision numpy scikit-learn matplotlib tqdm Pillow scikit-image




If a model already exists in models/, it will be loaded.

Otherwise, a new model is trained with augmented CIFAR-10 images.

After training, the script will display side-by-side comparisons of:

Original RGB

Grayscale input

Colorized output

🖼️ Visualization

Example layout:

[ Original ]   [ Grayscale ]   [ Colorized ]

📌 Notes

Training on CPU works but is slower. GPU is recommended.

Trained model is saved at:

.../models/colorization_model_full.pth

../models/colorization_model_full_weights.pth

The script is modular and can be adapted to other datasets.