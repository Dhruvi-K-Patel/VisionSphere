# VisionSphere: AI-Powered 2D & 3D Spatial Object Detection  

## Table of Contents  
1. [Project Overview](#project-overview)  
2. [Key Features](#key-features)  
3. [Technology Stack](#technology-stack)   
4. [Usage Instructions](#usage-instructions)  
5. [2D Spatial Object Detection](#2d-spatial-object-detection)  
6. [3D Spatial Object Annotation](#3d-spatial-object-annotation)  
7. [Future Enhancements](#future-enhancements)  
8. [Conclusion](#conclusion)  

---

## Project Overview  
**VisionSphere** is an AI-powered **2D and 3D spatial object detection system** that leverages **Google Gemini AI** for image processing. It automates the detection of objects in **2D images** and marks spatial points in **3D scenes**, providing valuable insights into object localization and classification.

The project consists of two main components:
1. **2D Spatial Object Detection** – Identifies and draws bounding boxes around objects in images.
2. **3D Spatial Object Annotation** – Marks specific points of interest in 3D images with labels.

---

## Key Features  
✅ **2D Bounding Box Detection** – Detects objects in images and draws labeled bounding boxes.  
✅ **3D Point Annotation** – Identifies important features and marks them on 3D objects.  
✅ **Google Gemini AI Integration** – Uses AI models for object detection and classification.  
✅ **Automated Image Processing** – Downloads and processes images dynamically.  
✅ **Customizable Parameters** – Adjust detection accuracy, bounding box limits, and visualization.  

---

## Technology Stack  
- **Programming Language**: Python  
- **AI Framework**: Google Gemini AI  
- **Libraries**:  
  - `PIL` (Python Imaging Library) for image processing  
  - `google-genai` for AI model interactions  
  - `requests` for image downloading  
  - `json` for object annotation  

---

## Usage Instructions

### 1. 2D Spatial Object Detection
- Run `2D_spatial.ipynb` in Jupyter Notebook.
- Upload an image or use a pre-downloaded image.
- The AI model will detect objects and draw bounding boxes.
- The processed image will be displayed with detected objects.

### 2. 3D Spatial Object Annotation
- Run `3D_spatial.ipynb` in Jupyter Notebook.
- Download sample 3D images using the provided script.
- The AI model will analyze and mark points of interest in the 3D image.
- The results will be visualized with labeled annotations.

## 2D Spatial Object Detection
This component detects objects in 2D images using Google's Gemini AI.

### How It Works
- The AI receives an image and returns object bounding boxes in JSON format.
- The system then plots these bounding boxes on the image with labels.

### Example Output Format (JSON)
```json
[
    {"label": "car", "box_2d": [100, 200, 300, 400]},
    {"label": "person", "box_2d": [50, 150, 250, 350]}
]
```

### Visualization
The processed image will highlight detected objects with color-coded bounding boxes and labels.

## 3D Spatial Object Annotation
This component analyzes 3D images and marks key features such as objects, tools, and landmarks.

### How It Works
- The AI takes a 3D image as input.
- It processes the image and returns labeled points of interest.
- The system plots these points on the image for visualization.

### Example Output Format (JSON)
```json
[
    {"point": [396, 628], "label": "screw"},
    {"point": [406, 517], "label": "screw"},
    {"point": [481, 754], "label": "handle"}
]
```

### Visualization
The system overlays detected points onto the 3D image with labels for each feature.

## Future Enhancements
✅ **Support for More Object Categories** – Expand detection to complex objects.
✅ **Real-Time Video Processing** – Extend functionality to video streams.
✅ **3D Mesh Processing** – Detect objects on 3D meshes and point clouds.
✅ **Web Interface** – Provide an interactive GUI for users.

## Conclusion
**VisionSphere** is an advanced AI-powered object detection system that brings automation to 2D and 3D image processing. By integrating Google Gemini AI, it ensures high accuracy and efficiency in object recognition.
