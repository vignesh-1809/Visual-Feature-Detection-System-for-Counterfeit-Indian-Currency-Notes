### Project Overview

This project focuses on identifying counterfeit Indian currency notes by analyzing visual features through image processing. It leverages techniques such as ORB (Oriented FAST and Rotated BRIEF) for feature detection and SSIM (Structural Similarity Index) for image comparison.

### Key Features

* **Image Acquisition**: Captures images of currency notes using digital cameras or scanners.
* **Pre-processing**: Resizes images, converts them to grayscale, and applies Gaussian blurring to reduce noise.
* **Feature Detection and Matching**:

  * *Security Thread*: Uses ORB to detect key features like the security thread.
  * *Bleed Lines*: Detects the presence and count of angular bleed lines in ₹500 and ₹2000 notes.
  * *Number Panel*: Verifies the number of characters in the serial number panel.
* **Image Analysis**: Compares extracted features using SSIM to determine the authenticity of the currency.
* **GUI**: Provides a user-friendly interface built with Tkinter, allowing users to upload images and receive instant validation results.([GitHub][1])

### Methodology

The system follows a structured process involving image acquisition, preprocessing, feature extraction, and analysis using a combination of ORB and SSIM techniques. It validates security features like latent images, watermarks, security threads, and Mahatma Gandhi's portrait, checks bleed lines, and verifies the number panel.

### Results

* **Accuracy**:

  * *Real Notes*: Achieved 79% accuracy based on testing of ₹500 and ₹2000 notes.
  * *Fake Notes*: Achieved 83% accuracy based on testing of counterfeit notes of the same denominations.
* **Performance**: Processes each note in approximately 5 seconds when only final results are displayed, making it a quick and efficient solution for counterfeit detection.

### Technologies and Libraries Used

* **Programming Language**: Python
* **Development Environment**: Jupyter Notebook
* **Libraries**:

  * OpenCV: For image processing and computer vision tasks
  * Tkinter: For creating the graphical user interface (GUI)
  * SSIM (Structural Similarity Index): For image comparison
  * ORB (Oriented FAST and Rotated BRIEF): For feature extraction and matching
  * NumPy: For numerical computation
  * Matplotlib: For visualization and analysis
  * Scikit-image: For SSIM-based similarity scoring([IJRASET][2],
