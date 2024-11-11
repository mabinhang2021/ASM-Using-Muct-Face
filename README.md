# Active Shape Model Using MUCT Dataset

This project implements an Active Shape Model (ASM) for facial landmark detection using the MUCT face database.

## Overview

The Active Shape Model learns facial shape variations from a training set and can generate new face shapes. The implementation includes:

- Mean shape calculation
- Shape alignment using Procrustes Analysis
- PCA-based shape variation modeling
- Visualization of different shape variations

## Features

### Shape Variations
The model shows three types of shape variations:
1. **Mean Shape**: The average face shape from training data
2. **Component Variations**: Shows how faces vary along principal components
3. **Random Shapes**: Generates possible face shapes by combining variations

### Visualization
The project includes visualization tools that show:
- Mean face shape (green points)
- First three component variations (different colors)
- Multiple random shape variations
- Comparisons between different variation types

## Installation
bash
Clone the repository
git clone https://github.com/mabinhang2021/ASM-Using-Muct-Face.git

## Usage

(1)Download  full MUCT Dataset
1. Visit the [MUCT Database](https://github.com/StephenMilborrow/muct)
2. Download required files:
   - `muct-landmarks-v1.csv` (landmark coordinates)
   - `muct-*.jpg` (face images)
3. Place downloaded files in your project directory:
muct-data/
│ ├── muct-landmarks.zip
│ └── muct-images.zip

(2)Run the file in ASM/using muct face.py
## Results

The model demonstrates:
- Successful alignment of face shapes
- Clear visualization of shape variations
- Effective PCA-based shape modeling
![Snipaste_2024-11-11_19-57-36](https://github.com/user-attachments/assets/0a5fd431-0304-4073-b484-06a1b12888c5)
![Snipaste_2024-11-11_19-57-47](https://github.com/user-attachments/assets/7bb388d5-88ac-457d-83cf-25aee0d666dd)



### Understanding the Visualizations
The visualization shows three types of shape variations:
1. **Mean Shape** (Green points)
   - Average face shape from training data
   - Baseline for comparing variations

2. **Component Variations** (Red, Blue, Yellow points)
   - First three principal components
   - Shows main ways faces vary in dataset

3. **Random Shapes** (Multiple colors)
   - Different possible face shapes
   - Combines multiple variations


## Dependencies
- Python 3.7+
- NumPy
- OpenCV
- Matplotlib
- SciPy
- Scikit-learn

## Important Notes
- The MUCT dataset is not fully included in this repository
- You need to download it separately from [MUCT Database](https://github.com/StephenMilborrow/muct)
- Make sure to place the dataset files in the correct directory structure
- If interested in more information about ASM, please pay attention to this repository, I will add some paper interpretation and pre-mathematical knowledge in the future, thank you


## Acknowledgments
- [MUCT Database](https://github.com/StephenMilborrow/muct) for providing the face dataset
