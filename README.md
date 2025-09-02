# Image Colorization Project

This repository contains experiments and implementations related to **image colorization** using deep learning techniques.  
The project is divided into multiple tasks, each focusing on a different approach or challenge in colorization.

---

## 📂 Project Structure
├── requirements.txt # Python dependencies
├── README.md # Project documentation
├── Task1 # Experiment with various loss functions
├── Task2 # Artistic Style Transfer in Colorization
├── Task3 # Conditional Image Colorization
├── Task4 # Dataset Augmentation for Colorization
├── models # Trained models and architectures ( google drive link :https://drive.google.com/drive/folders/1P1pxTWWQTITh0YSBCg8rvqfIACDBxL-L?usp=drive_link
  paste every model files inside this folder)
└── data # Datasets used for training and testing (automatically downloaded when u run task1)



---

## 📝 Tasks

### **Task 1: Experiment with Various Loss Functions**
- **Description**: Experiment with different loss functions (e.g., Mean Squared Error, Perceptual Loss) to compare their effect on colorization quality.
- **Guidelines**:
  - Use the same model architecture and dataset.
  - Only modify the loss function.
  - Compare results and explain differences.
  - GUI is **not required**.

---

### **Task 2: Artistic Style Transfer in Colorization**
- **Description**: Colorize grayscale photos while simultaneously applying a chosen artistic style.
- **Guidelines**:
  - Combine **image colorization** with **style transfer**.
  - Allow users to choose from a set of artistic styles.
  - A **graphical user interface (GUI)** should be implemented for:
    - Uploading images
    - Selecting styles

---

### **Task 3: Conditional Image Colorization**
- **Description**: Colorize grayscale photos based on **user-defined conditions** (e.g., sky should be blue, grass should be green).
- **Guidelines**:
  - Enable user input for color preferences.
  - Support selecting or entering color criteria for specific regions.
  - A **GUI** should be implemented to support this interaction.

---

### **Task 4: Dataset Augmentation to Improve Colorization**
- **Description**: Improve colorization results by applying dataset augmentation techniques such as:
  - Rotation
  - Flipping
  - Brightness alterations
- **Guidelines**:
  - Train models on both original and augmented datasets.
  - Compare results before and after augmentation.
  - GUI is **not required**, but provide comparative results.

---

## 📦 Installation
To install dependencies, run:
```bash
pip install -r requirements.txt
📊 Results
Each task folder will contain:

Code implementations

Models

Output results (comparisons, visualizations)

Results and comparisons are documented within respective task folders.