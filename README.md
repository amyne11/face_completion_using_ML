# Face Recognition and Completion Using Machine Learning

This project implements face recognition and completion tasks using machine learning techniques. The dataset includes face images of 40 subjects, with 10 images per subject, each having 32x32 pixels and 256 grey levels per pixel.

## Table of Contents
- [Introduction](#introduction)
- [Approach](#approach)
- [Future Work](#future-work)
- [Contributing](#contributing)

## Introduction
This project aims to recognize and complete faces using L2-regularized least squares for classification and regression tasks. The provided dataset includes 400 images of faces, split into training and test sets.

## Approach

### Face Recognition

**Data Preparation:**
- Loaded data and labels using custom functions.
- Normalized pixel values to [0, 1].
- Partitioned data into training and test sets with a 5:5 split per subject.

**Model Training:**
- Implemented L2-regularized least squares (L2-RLS) for multi-class classification.
- Used hyperparameter selection to choose the best lambda value.

**Evaluation:**
- Evaluated model accuracy using a confusion matrix.
- Visualized correctly and incorrectly classified faces.

### Face Completion

**Data Preparation:**
- Split faces into left and right halves.
- Used left half to predict the right half.

**Model Training:**
- Trained an L2-RLS model with lambda set to 0 for regression.

**Evaluation:**
- Evaluated model performance using Mean Absolute Percentage Error (MAPE).
- Visualized and compared ground truth and completed faces.

## Future Work
- Expand the dataset for better robustness.
- Develop a real-time face recognition system.
- Explore advanced architectures and techniques like transfer learning.

## Contributing
Contributions are welcome! Please submit a pull request or open an issue for suggestions or improvements.

