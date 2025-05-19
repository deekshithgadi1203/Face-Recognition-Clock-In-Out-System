Face Recognition Attendance System
This is a Python-based application built using Tkinter for the GUI, OpenCV for face detection, and DeepFace for face recognition. It allows users to register their faces, log in using face recognition, and maintain attendance logs.

Features

User Registration:
New users can register by capturing their face and providing a username.
Embeddings of the captured face are computed using DeepFace and stored in a .pickle file for future recognition.

Login:
Users can log in by scanning their face using a webcam.
If the face is recognized, a welcome message is displayed, and the login details are saved in a log file.
If the face is not recognized, an error message is displayed, prompting the user to register.
Webcam Integration:

The application captures real-time video frames using OpenCV and displays them in the GUI.
Detected faces are highlighted with red rectangles.

Face Recognition:
Uses Facenet (via DeepFace) to compute face embeddings and compare them against registered embeddings.
The recognition is based on cosine similarity.

Attendance Log:
Successful logins are recorded in a log.txt file with the username and timestamp.
