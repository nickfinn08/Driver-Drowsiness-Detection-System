# Drowsiness Detection System using OpenCV, dlib, and Pygame
Driver Drowsiness Detection System is a real time project that uses python libraries like OpenCV, NumPy, pygame, dlib and imutils that monitors the eyes of the driver. Based on real time calculations if found equal to sleeping it sets on an alarm to alert the user after a while of closing eyes.

# Features
1.Real-time video processing using webcam.  
2.Facial and eye landmark detection.  
3.Drowsiness classification based on eye aspect ratio (EAR).  
4.Alarm system for sleep detection
# How It Works:
1.The webcam captures a live feed.  
2.dlib detects facial landmarks, particularly eye landmarks.  
3.The blinked function calculates the eye aspect ratio (EAR):  
4.A high EAR implies open eyes (Active)  
5.A medium EAR indicates partial closure (Drowsy)  
6.A low EAR implies fully closed eyes (Sleeping)  
7.Based on the EAR over a number of frames, the script categorizes the user's alertness.  
8.If the user is sleeping, an alarm is played using pygame.  

# Required libraries and their roles:
1.OpenCV is used access the webcam which process images and draws overlays. It also converts color space to grayscale for more efficient face detection.  
2.NumPy is used for numerical computations, especially distance calculations between facial landmarks.  
3.dlib Performs facial detection and loads a pre-trained facial landmark model to identify 68 facial points. It is ssential for accurately detecting eye positions that returns the right output.  
4.Imutils simplifies conversions and manipulations of dlib shape objects. face_utils.shape_to_np converts dlib landmarks to NumPy arrays for easier manipulation.  
5.Finally pygame handles the audio playback for alarm when sleep is detected.  
