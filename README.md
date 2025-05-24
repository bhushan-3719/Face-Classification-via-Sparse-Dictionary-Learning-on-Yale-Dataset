# Face-Classification-via-Sparse-Dictionary-Learning-on-Yale-Dataset
This project implements a face classification and novelty detection system using sparse dictionary learning. It was developed as part of a Machine Learning course and tested on the Yale Face Database with 100% accuracy on 19 test images.


Project Highlights
Used Dataset: Yale Face Database (Grayscale Images)

Approach: Sparse Dictionary Learning with class-wise atom mapping

Optimization: Solved using CVXPY to separate signal from noise

Result: 100% accuracy on 19 test images with precise classification and robust novelty detection

Technologies Used
Python 3

OpenCV (for image processing)

NumPy

Scikit-learn (for dictionary learning)

CVXPY (for convex optimization)

Matplotlib (for visualization)

Preprocessing: Load grayscale face images and resize to 64×64.

Training: Learn a dictionary and sparse representations (codes) for training images using DictionaryLearning.

Classification: For each test image:

Reconstruct it using sparse codes

Minimize error: x = Dα + e via convex optimization

Assign class based on residual error across learned atoms

Visualization: Plot sparse codes, test image, reconstructed image, and error heatmap.
