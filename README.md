# Drowsiness Detection System using OpenCV, dlib, and Pygame
Driver Drowsiness Detection System is a real time project that uses python libraries like OpenCV, NumPy, pygame, dlib and imutils that monitors the eyes of the driver. Based on real time calculations if found equal to sleeping it sets on an alarm to alert the user after a while of closing eyes.

# Features
Real-time video processing using webcam.
Facial and eye landmark detection.
Drowsiness classification based on eye aspect ratio (EAR).

Alarm system for sleep detection
# How It Works:
The webcam captures a live feed.
dlib detects facial landmarks, particularly eye landmarks.
The blinked function calculates the eye aspect ratio (EAR):
A high EAR implies open eyes (Active)
A medium EAR indicates partial closure (Drowsy)
A low EAR implies fully closed eyes (Sleeping)
Based on the EAR over a number of frames, the script categorizes the user's alertness.
If the user is sleeping, an alarm is played using pygame.

# Required libraries and their roles:
OpenCV is used access the webcam which process images and draws overlays. It also converts color space to grayscale for more efficient face detection.
NumPy is used for numerical computations, especially distance calculations between facial landmarks.
dlib Performs facial detection and loads a pre-trained facial landmark model to identify 68 facial points. It is ssential for accurately detecting eye positions that returns the right output.
Imutils simplifies conversions and manipulations of dlib shape objects. face_utils.shape_to_np converts dlib landmarks to NumPy arrays for easier manipulation.
Finally pygame handles the audio playback for alarm when sleep is detected.
