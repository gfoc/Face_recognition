# Face_recognition

This project uses a face recognition-based attendance system that leverages OpenCV for face detection and a K-Nearest Neighbors (KNN) classifier to identify individuals. It uses a live video feed from the webcam to detect faces with the Haar Cascade Classifier. Once a face is detected, the region of interest is extracted, resized, and fed into the KNN model, which has been trained on pre-saved face data and corresponding labels. 

This Project has 3 files.
1. Attendance
2. Dataset
3. haarcascade_frontalface_default.xml


haarcascade_frontalface_default.xml is a pre-trained model file used by OpenCV for face detection. It is part of the Haar Cascade classifier, a machine-learning object detection algorithm designed to identify objects in images specifically faces in this case.

Haar Features: The Haar Cascade algorithm uses Haar-like features, essentially combinations of pixel intensities that are checked in different areas of the image.
Training: The model in haarcascade_frontalface_default.xml has been trained using thousands of positive (face) and negative (non-face) images to recognize patterns typical of human faces.
Detection: When you use this file in your project, OpenCV applies these learned patterns to the input image or video frame to detect faces. It does this by scanning the image at multiple scales and positions to find the best match for a face.
