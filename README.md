

---

# 🖼️ **Shape and Color Detection with Computer Vision**

This repository demonstrates tasks in computer vision using **OpenCV** and **Python**, focusing on detecting shapes, computing areas, identifying traffic signals, and segmenting shapes based on color. Each task is modularized into subprograms to ensure clarity and flexibility. 🚀

---

## 📂 **Repository Structure**

```plaintext
├── Detailed-Observations.docx   # Comprehensive documentation of observations
├── README.md                    # Project documentation
├── Shape_Recognition_and_Color_Segmentation.ipynb  # Jupyter notebook for all subprograms
├── images/                      # Contains task output images
│   ├── Task1.1.png
│   ├── Task1.2.png
│   ├── Task1.3.png
│   ├── Task2.png
│   ├── Task3-1.png
│   ├── Task3-2.png
│   ├── Task3-3.png
│   ├── Task4-1.png
│   ├── Task4-2.png
│   ├── Task4-3.png
│   ├── Task4-4.png
│   ├── Task4-5.png
│   ├── Task4-6.png
│   ├── Task4-7.png
│   ├── Task4-8.1.png
│   ├── Task4-8.png
│   └── ...
```

---

## 🛠️ **Features Implemented**

This project consists of **8 key subprograms**:

1. ✨ **Subprogram 1: Detect Shape Coordinates and Display**  
2. ✨ **Subprogram 2: Compute Shape Areas**  
3. 🎯 **Subprogram 3: Detect Only Red Circles**  
4. 🌿 **Subprogram 4: Detect All Green Shapes**  
5. 🌟 **Subprogram 5: Detect Large Circles**  
6. 🔴 **Subprogram 6: Detect Small Circles**  
7. ✨ **Subprogram 7: Detect and Count Corners**  
8. 📸 **Subprogram 8: Shape Segmentation and Display**

---

## 📖 **Subprograms Overview**

---

### ✨ **Subprogram 1: Detect Shape Coordinates and Display**
- **Objective:** Identify all shapes in the image and determine their centroids (geometric center).
- **Method:**  
  1. Convert the input image to grayscale and apply binary thresholding.  
  2. Use `cv2.findContours` to detect contours.  
  3. Calculate centroids using image moments (`cv2.moments`).  
  4. Overlay the centroids on the image as `(x, y)` coordinates.  

📷 **Output Example:**  
- Shapes with their respective centroids:  
  ![Task1.1](images/Task1.1.png)  
  ![Task1.2](images/Task1.2.png)  
  ![Task1.3](images/Task1.3.png)  

**Use Cases:**  
- Analyzing the spatial distribution of objects in an image.  
- Robotic arm path planning.

---

### ✨ **Subprogram 2: Compute Shape Areas**
- **Objective:** Compute the area of each detected shape and annotate the image with the calculated values.  
- **Method:**  
  1. Detect contours using the same method as Subprogram 1.  
  2. Calculate the area of each contour using `cv2.contourArea`.  
  3. Overlay the computed area near each shape for visualization.  

📷 **Output Example:**  
- Shape areas displayed:  
  ![Task2](images/Task2.png)  

**Use Cases:**  
- Object size analysis for quality control in manufacturing.  
- Estimation of surface area in aerial imagery.

---

### 🎯 **Subprogram 3: Detect Only Red Circles**
- **Objective:** Filter and highlight only red circles in the image.  
- **Method:**  
  1. Convert the image to HSV color space.  
  2. Create masks for two red hue ranges (due to HSV's split red representation).  
  3. Apply the Hough Circle Transform (`cv2.HoughCircles`) to detect circles in the masked image.  
  4. Highlight detected red circles with bounding circles.  

📷 **Output Example:**  
- Red circles detected and highlighted:  
  ![Task3-1](images/Task3-1.png)  
  ![Task3-2](images/Task3-2.png)  
  ![Task3-3](images/Task3-3.png)  

**Use Cases:**  
- Traffic light detection in autonomous vehicles.  
- Identifying warning signals in surveillance systems.

---

### 🌿 **Subprogram 4: Detect All Green Shapes**
- **Objective:** Detect all shapes filled with green color.  
- **Method:**  
  1. Convert the image to HSV color space.  
  2. Create a mask for green hues.  
  3. Detect contours in the masked image and highlight the shapes.  

📷 **Output Example:**  
- Green shapes highlighted:  
  ![Task4-1](images/Task4-1.png)  
  ![Task4-2](images/Task4-2.png)  
  ![Task4-3](images/Task4-3.png)  
  ![Task4-4](images/Task4-4.png)  
  ![Task4-5](images/Task4-5.png)  
  ![Task4-6](images/Task4-6.png)  
  ![Task4-7](images/Task4-7.png)  
  ![Task4-8.1](images/Task4-8.1.png)  
  ![Task4-8](images/Task4-8.png)  

**Use Cases:**  
- Environmental monitoring (detecting vegetation in satellite images).  
- Sports analytics (e.g., identifying field markings).

---

### 🌟 **Subprogram 5: Detect Large Circles**
- **Objective:** Detect circles above a specified radius threshold.  
- **Method:**  
  1. Convert the image to grayscale.  
  2. Apply the Hough Circle Transform with a large radius threshold to isolate large circles.  

📷 **Output Example:**  
- Large circles detected:  
  ![Task5](images/Task5.png)  

**Use Cases:**  
- Identifying circular structures in construction or design plans.  
- Detecting planets or craters in astronomical images.

---

### 🔴 **Subprogram 6: Detect Small Circles**
- **Objective:** Detect circles below a specified radius threshold.  
- **Method:**  
  1. Follow the same process as Subprogram 5 but adjust the radius threshold for smaller circles.  

📷 **Output Example:**  
- Small circles detected:  
  ![Task6](images/Task6.png)  

**Use Cases:**  
- Detecting small objects like coins in sorting machines.  
- Particle size analysis in materials research.

---

### ✨ **Subprogram 7: Detect and Count Corners**
- **Objective:** Detect distinct corners of all shapes in the image.  
- **Method:**  
  1. Use the Harris Corner Detection method (`cv2.goodFeaturesToTrack`) to find corners.  
  2. Highlight corners on the image.  

📷 **Output Example:**  
- Corners detected and marked:  
  ![Task7](images/Task7.png)  

**Use Cases:**  
- Edge detection in 3D modeling.  
- Feature extraction in image registration.

---

### 📸 **Subprogram 8: Shape Segmentation and Display**
- **Objective:** Segment individual shapes, save them as separate files, and overlay them with highlights for visualization.  
- **Method:**  
  1. Detect contours and extract bounding rectangles for each shape (`cv2.boundingRect`).  
  2. Crop the shape regions and save them as separate image files.  
  3. Visualize the segmentation by overlaying the shapes with unique highlights.  

📷 **Output Example:**  
- Segmented shapes visualized:  
  ![Task8](images/Task8.png)  

**Use Cases:**  
- Dataset creation for machine learning models.  
- Isolating objects in medical imaging (e.g., tumors in X-rays).

---

## 🚀 **How to Use**

1. **Clone the repository:**  
   ```bash
   git clone https://github.com/your-username/Shape-Color-Detection-CV.git
   ```
2. **Install dependencies:**  
   ```bash
   pip install opencv-python numpy matplotlib
   ```
3. **Run the Jupyter notebook:**  
   ```bash
   jupyter notebook Shape_Recognition_and_Color_Segmentation.ipynb
   ```
4. **Explore detailed outputs:** Check `Detailed-Observations.docx` for explanations.

---

## 🛠️ **Technologies Used**

- **Python** 🐍  
- **OpenCV** 🖼️  
- **Numpy** 🔢  
- **Matplotlib** 📊  

---

## 🙌 **Contributions**

Contributions are welcome! Whether it's reporting bugs, suggesting features, or improving the code, feel free to open an issue or submit a pull request.
