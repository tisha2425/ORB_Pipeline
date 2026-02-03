# Computer Vision Pipeline using OpenCV

This project demonstrates a complete computer vision workflow.
Vou process an image from capture to final object detection.
The pipeline uses OpenCV and classical vision techniques.

---

## Project Overview

Vou perform the following tasks.

• Image capture and preprocessing  
• Segmentation and ROI extraction  
• Feature extraction using ORB  
• Feature matching between images  
• Rule based object classification  
• Post processing using Non Maximum Suppression  

This project focuses on understanding how classical computer vision works step by step.

---

## Technologies Used

• Python  
• OpenCV  
• NumPy  
• Matplotlib  

---

## Pipeline Steps

### Step 1. Image Capture and Preprocessing

• Capture image from webcam or load from disk  
• Convert image to grayscale  
• Reduce noise using Gaussian blur  
• Enhance contrast using histogram equalization  

Output  
`preprocessed.jpg`

---

### Step 2. Segmentation and ROI

• Apply binary thresholding  
• Separate foreground from background  
• Detect external contours  
• Visualize segmented regions  

Output  
`segmented.jpg`

---

### Step 3. Feature Extraction

• Load segmented image  
• Detect keypoints using ORB  
• Compute binary descriptors  
• Visualize feature locations  

Output  
`features.jpg`

---

### Step 4. Feature Matching

• Extract ORB features from two images  
• Match descriptors using Hamming distance  
• Sort matches by similarity  
• Display strongest matches  

Purpose  
Compare visual similarity between images.

---

### Step 5. ML Based Object Classification

• Detect objects using contours  
• Use contour area as a feature  
• Classify objects as Small or Large  
• Visualize classification results  

This is a simple rule based ML approach.

---

### Step 6. Post Processing with NMS

• Take detected bounding boxes  
• Remove overlapping detections  
• Keep highest confidence boxes  
• Display final output  

This improves detection quality.

---

## How to Run

1. Install dependencies  
```bash
pip install opencv-python numpy matplotlib
