# FaceFinder AI

*FaceFinder AI* is a Python-based face recognition project that uses a trained deep learning model and Haar cascade classifier to detect and classify faces in real-time using a webcam or IP camera.

---

## Features

- Real-time face detection and recognition using webcam/IP camera
- Preprocessing for consistent input to the trained model
- Easily expandable to add more users
- Displays recognized names on screen

---

## Project Structure


facefinderAI/

├── data/
│   ├── images/
│   └── labels/

├── collect_data (1).py      # For collecting training data

├── consolidated_data (1).py # For processing dataset

├── face.h5                  # Trained model (not included)

├── face_detect.py           # Basic face detection

├── haarscascade_frontalface_default (1).xml # Haar Cascade XML

├── recognize.py             # Main recognition script


---

## Requirements

Install dependencies using pip:

bash
pip install opencv-python numpy keras tensorflow


---

## How to Use

### 1. Webcam/IP Camera Setup

Edit the URL in recognize.py to point to your webcam or IP camera stream:

python
URL = "http://192.168.158.127:8080/shot.jpg"


Make sure your mobile or camera app supports MJPEG or JPEG snapshot streaming.

---

### 2. Add Labels

Edit the labels list inside recognize.py to reflect the people you've trained the model on:

python
labels = ['X', 'Y', 'Z', 'unknown']


Make sure these correspond to your training data in the correct order.

---

### 3. Run the Recognition Script

bash
python recognize.py


It will open a window showing the real-time video feed with recognized names labeled on faces.

---

## Model Info

The trained model file (face.h5) is *not included* in this repository due to its large size.

*If you would like to get the trained model, please contact me at:*

**sampritapatra123@gmail.com**

---

## Notes

- Ensure that haarscascade_frontalface_default.xml is present in the root folder.
- For training, use collect_data (1).py and consolidated_data (1).py to gather and prepare dataset images.
- The model was trained using Keras with CNN architecture for face classification.

---

## License

This project is for educational purposes. You can modify and use it for personal projects.

---

## Author

Developer of FaceFinder AI - Samprita 
---
Contact: sampritapatra123@gmail.com
---
