
---

# 🖼️ **Shape and Color Detection with Computer Vision**

This repository showcases tasks in computer vision, focusing on detecting shapes, computing areas, analyzing traffic signals, and segmenting shapes based on colors. 🚀

---

## 📂 **Repository Structure**

```plaintext
├── Detailed-Observations.docx   # Detailed documentation of the observations
├── README.md                    # Project documentation
├── Shape_Recognition_and_Color_Segmentation.ipynb  # Jupyter notebook for all tasks
├── images/                      # Contains all task output images
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
│   ├── Task4-8.png
│   ├── Task4-8.1.png
```

---

## 🛠️ **Features Implemented**

This project includes the following key tasks:

1. 🔍 **Detect Shape Coordinates**  
2. 📐 **Compute Shape Areas**  
3. 🚦 **Traffic Signal Detection**  
4. 🟢 **Shape and Color Detection (8 Subtasks)**  

---

## 📖 **Tasks Overview**

---

### 📝 **Task 1: Detect Shape Coordinates**  
Detect and calculate the centroids of shapes in the image. The centroids are output as `(x, y)` coordinates.  

📷 **Output:**  
![Task 1.1](images/Task1.1.png)  
[Task 1.1](images/Task1.1.png)  

---

### 📝 **Task 2: Compute Shape Areas**  
Compute the area of each detected shape using contours.  

📷 **Output:**  
![Task 2](images/Task2.png)  
[Task 2](images/Task2.png)  

---

### 📝 **Task 3: Traffic Signal Detection**  
Analyze a traffic signal image and identify the active signal (red, yellow, or green).  

📷 **Outputs:**  
- **Red Signal Active:**  
  ![Task 3-1](images/Task3-1.png)  
  [Task 3-1](images/Task3-1.png)  

- **Yellow Signal Active:**  
  ![Task 3-2](images/Task3-2.png)  
  [Task 3-2](images/Task3-2.png)  

- **Green Signal Active:**  
  ![Task 3-3](images/Task3-3.png)  
  [Task 3-3](images/Task3-3.png)  

---

### 📝 **Task 4: Shape and Color Detection**  
Detect geometric properties of shapes, corners, and color-based regions. This task includes eight subtasks:  

---

#### **Task 4.1: Detect Large Circles**  
Detect circles with a radius above a certain threshold.  

📷 **Output:**  
![Task 4-1](images/Task4-1.png)  
[Task 4-1](images/Task4-1.png)  

---

#### **Task 4.2: Detect Small Circles**  
Detect circles with a radius below a certain threshold.  

📷 **Output:**  
![Task 4-2](images/Task4-2.png)  
[Task 4-2](images/Task4-2.png)  

---

#### **Task 4.3: Detect Corners**  
Detect corners of all shapes using the Harris Corner Detection method.  

📷 **Output:**  
![Task 4-3](images/Task4-3.png)  
[Task 4-3](images/Task4-3.png)  

---

#### **Task 4.4: Detect Red Circles**  
Detect and highlight red-colored circles.  

📷 **Output:**  
![Task 4-4](images/Task4-4.png)  
[Task 4-4](images/Task4-4.png)  

---

#### **Task 4.5: Detect Green Shapes**  
Detect and highlight all green-colored shapes.  

📷 **Output:**  
![Task 4-5](images/Task4-5.png)  
[Task 4-5](images/Task4-5.png)  

---

#### **Task 4.6: Color Simplification**  
Simplify the image by retaining only red, yellow, green, and blue colors.  

📷 **Output:**  
![Task 4-6](images/Task4-6.png)  
[Task 4-6](images/Task4-6.png)  

---

#### **Task 4.7: Shape Segmentation**  
Segment individual shapes from the image and save them as separate files.  

📷 **Output:**  
![Task 4-7](images/Task4-7.png)  
[Task 4-7](images/Task4-7.png)  

---

#### **Task 4.8: Highlight Segmented Shapes**  
Visualize segmented shapes together and highlight each one.  

📷 **Outputs:**  
![Task 4-8](images/Task4-8.png)  
[Task 4-8](images/Task4-8.png)  

![Task 4-8.1](images/Task4-8.1.png)  
[Task 4-8.1](images/Task4-8.1.png)  

---

## 🚀 **How to Use**

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/Shape-Color-Detection-CV.git
   ```
2. Install dependencies:  
   ```bash
   pip install opencv-python numpy
   ```
3. Open and run the `Shape_Recognition_and_Color_Segmentation.ipynb` notebook.  
4. View the detailed observations in `Detailed-Observations.docx`.

---

## 🛠️ **Technologies Used**
- **Python** 🐍  
- **OpenCV** 🖼️  
- **Numpy** 🔢  

---

## 🙌 **Contributions**  
Contributions are welcome! Feel free to open an issue or create a pull request.  

---
