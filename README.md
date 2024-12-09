# 🖼️ **Shape and Color Detection with Computer Vision**

This repository demonstrates tasks in computer vision, focusing on detecting shapes, computing areas, analyzing traffic signals, and segmenting shapes based on their colors. 🚀 Each task is broken into subprograms for modularity and better understanding.

---

## 📂 **Repository Structure**

```plaintext
├── Detailed-Observations.docx   # Comprehensive documentation of observations
├── README.md                    # Project documentation
├── Shape_Recognition_and_Color_Segmentation.ipynb  # Jupyter notebook for all subprograms
├── images/                      # Contains task output images
│   ├── Task1.1.png
│   ├── Task1.2.png
│   ├── Task2.png
│   ├── Task3-1.png
│   ├── Task4-1.png
│   ├── Task5.png
│   └── ...
```

---

## 🛠️ **Features Implemented**

This project includes eight subprograms:

1. ✨ **Subprogram 1: Detect Shape Coordinates and Display**  
2. ✨ **Subprogram 2: Compute Area**  
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
This subprogram identifies shapes in an image and calculates their centroids. Centroids are displayed as `(x, y)` coordinates overlaid on the shapes.

📷 **Output Examples:**  
- ![Task 1.1](images/Task1.1.png)  
- ![Task 1.2](images/Task1.2.png)  

---

### ✨ **Subprogram 2: Compute Area**
The program computes the areas of detected shapes using contour analysis. Each area is displayed over its respective shape in the image.

📷 **Output Example:**  
- ![Task 2](images/Task2.png)  

---

### 🎯 **Subprogram 3: Detect Only Red Circles**
This subprogram filters and highlights only red-colored circles in an image. Detection is performed using HSV masks and circle detection algorithms.

📷 **Output Example:**  
- ![Task 3](images/Task3-1.png)  

---

### 🌿 **Subprogram 4: Detect All Green Shapes**
Shapes filled with green color are detected and highlighted using HSV-based color masking.

📷 **Output Example:**  
- ![Task 4](images/Task4-1.png)  

---

### 🌟 **Subprogram 5: Detect Large Circles**
Large circles are detected based on their radius. Minimum and maximum thresholds are customizable to detect only circles of desired size.

📷 **Output Example:**  
- ![Task 5](images/Task5.png)  

---

### 🔴 **Subprogram 6: Detect Small Circles**
This program detects small circles by setting a radius threshold. Smaller circles are highlighted for easy identification.

📷 **Output Example:**  
- ![Task 6](images/Task6.png)  

---

### ✨ **Subprogram 7: Detect and Count Corners**
The Harris Corner Detection method is used to locate and count distinct corners in the detected shapes.

📷 **Output Example:**  
- ![Task 7](images/Task7.png)  

---

### 📸 **Subprogram 8: Shape Segmentation and Display**
This subprogram segments individual shapes from the image, saves them as separate files, and overlays each shape with a unique highlight for visualization.

📷 **Output Example:**  
- ![Task 8](images/Task8.png)  

---

## 🧑‍💻 **Implementation Details**

Here’s how each subprogram works:

1. **Detect Shape Coordinates (Subprogram 1)**  
   - **Technique:** Contour detection (`cv2.findContours`) is used to identify shapes. Centroids are calculated using image moments (`cv2.moments`).

2. **Compute Area (Subprogram 2)**  
   - **Technique:** Contour area calculation (`cv2.contourArea`) is applied on binary images.

3. **Detect Red Circles (Subprogram 3)**  
   - **Technique:** HSV masking for red color and Hough Circle Transform (`cv2.HoughCircles`) for circle detection.

4. **Detect Green Shapes (Subprogram 4)**  
   - **Technique:** HSV masking for green color isolates and highlights the green shapes.

5. **Detect Large Circles (Subprogram 5)**  
   - **Technique:** Similar to Subprogram 3 but with customizable radius thresholds for large circles.

6. **Detect Small Circles (Subprogram 6)**  
   - **Technique:** Small radius thresholds in Hough Circle Transform isolate smaller circles.

7. **Detect and Count Corners (Subprogram 7)**  
   - **Technique:** Harris Corner Detection (`cv2.goodFeaturesToTrack`) pinpoints corners for each shape.

8. **Shape Segmentation and Display (Subprogram 8)**  
   - **Technique:** Bounding rectangles (`cv2.boundingRect`) extract shapes. Segmented shapes are saved and visualized separately.

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
4. **View detailed observations:** Open `Detailed-Observations.docx`.

---

## 🛠️ **Technologies Used**

- **Python** 🐍  
- **OpenCV** 🖼️  
- **Numpy** 🔢  
- **Matplotlib** 📊  

---

## 🙌 **Contributions**

Contributions are welcome! Feel free to open an issue or submit a pull request to enhance the functionality of this repository.

--- 
