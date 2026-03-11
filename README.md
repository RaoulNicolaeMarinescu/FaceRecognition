# Face Recognition System

This project implements a **Face Recognition system** capable of detecting and identifying faces from images or live video streams using machine learning techniques.

The system detects faces, extracts distinctive features using deep learning models, and compares them with previously stored embeddings to determine the identity of the person.

This project was developed as part of the **"Principles and Models of Perception"** course at the **University of Milan**.

---

## Authors

* Antonio Hlibey
* Stefano Confuorto
* Raoul Nicolae Marinescu

---

## Project Overview

Face recognition is a biometric technology used to **identify or verify a person's identity by analyzing facial features**.
Modern approaches rely on **deep learning models and convolutional neural networks (CNNs)** capable of recognizing faces even under complex conditions. 

The system follows a typical face recognition pipeline consisting of several steps:

1. **Face Detection**
   The algorithm analyzes an image or video frame to locate faces and returns their spatial coordinates.

2. **Face Alignment**
   Detected faces are normalized using facial keypoints to correct rotations and perspective distortions.

3. **Face Embedding**
   Each aligned face is converted into a numerical vector (embedding) representing its distinctive features.

4. **Face Matching**
   The embedding is compared with those stored in a database using similarity measures (e.g., Euclidean distance or cosine similarity).
   If the distance is below a threshold, the identity is considered a match. 

---

## Technologies Used

* Python
* OpenCV
* Face Recognition library (based on **dlib**)
* NumPy
* Jupyter Notebook

These tools are used to detect faces, extract embeddings, and compare them to identify individuals in real time.

---

## Project Structure

Example structure of the repository:

```
FaceRecognition
│
├── Face_Recognition_Live.ipynb
├── Face_Recognition_Video.ipynb
│
├── presentation/
    ├── Face Recognition.pptx
    └── Face Recognition.pdf
```

* **Face_Recognition_Live.ipynb** → Face recognition using a live webcam stream
* **Face_Recognition_Video.ipynb** → Face recognition from video files
* **Presentation / PDF** → Project explanation and theoretical background

---

## Example Output

The system detects faces in real time and labels them with the recognized identity using bounding boxes and labels.

Example result:

* Faces detected in the frame
* Bounding box around each face
* Name displayed if the identity is recognized

---

## Applications

Face recognition technology is widely used in many real-world scenarios, including:

* Smartphone unlocking
* Airport and stadium access control
* Video surveillance systems
* Customer behavior analysis
* Automatic photo organization 

---

## Limitations

Face recognition systems may encounter difficulties in some situations:

* Poor lighting conditions
* Occlusions (glasses, masks, hats)
* Facial expressions or head movements
* Bias in training datasets affecting recognition accuracy across demographic groups 

---

## Possible Future Improvements

Future developments of the project may include:

* Continuous facial analysis in video streams
* Improved 3D face alignment
* Integration of thermal and depth data
* Adaptive systems capable of learning user changes over time 

---

## How to Run the Project

1. Clone the repository

```
git clone https://github.com/your-username/FaceRecognition.git
```

2. Install the required libraries

```
pip install opencv-python face-recognition numpy
```

3. Open the notebooks

```
jupyter notebook
```

4. Run the cells in:

* `Face_Recognition_Live.ipynb` for webcam recognition
* `Face_Recognition_Video.ipynb` for video recognition

