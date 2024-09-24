# Smart-Attendnce-System

## Project Overview
The *Smart Attendance System* uses face recognition technology to automate the process of recording attendance. This system captures images, detects faces, and verifies them against a trained dataset to mark attendance. It also includes features like automated email notifications to alert users about attendance updates.

## Features
- *Face Recognition*: Utilizes OpenCV's Haar Cascade Classifier to detect faces.
- *Image Capture*: Captures live images through the webcam and processes them for face detection.
- *Training Model*: Trains the face recognition model using stored images.
- *Automated Email*: Sends attendance alerts via email after successful recognition.
- *Real-time Detection*: Continuously verifies the camera feed to match faces against the trained dataset.

## File Structure
- auto_email_sender.py: Script to send automated emails after attendance is marked.
- default_haarcascade.xml: Pre-trained Haar Cascade Classifier XML file for face detection.
- face_recognition.py: Main script for recognizing faces using OpenCV.
- image_capture.py: Script for capturing images from the webcam and saving them.
- train_faces.py: Script to train the face recognition model using stored images.
- verify_camera.py: Real-time face verification through the webcam.
- README.md: Documentation for the project.

## Prerequisites
- Python 3.x
- OpenCV
- NumPy
- smtplib (for email notifications)

You can install all dependencies using:
bash
pip install -r requirements.txt

## Instructions to Run:
1. First, download or clone the project:
   bash
   git clone https://github.com/yourusername/Smart-Attendance-System.git
   cd Smart-Attendance-System
   
2. Import the project into your favorite IDE.
3. Create a Python environment:
   bash
   python -m venv env
   
4. Activate the environment:
   - On Windows:
     bash
     .\env\Scripts\activate
     
   - On macOS/Linux:
     bash
     source env/bin/activate
     
5. Install all the required packages:
   bash
   pip install opencv-contrib-python
   pip install numpy
   pip install pandas
   pip install Pillow
   pip install pytest-shutil
   pip install python-csv
   pip install yagmail
   

6. Change the email information as needed in auto_email_sender.py.

7. Run the project using the command line or your IDE's Run button:
   bash
   python main.py

---> Future Enhancements :
- Integrating with a cloud-based database for storing attendance logs.
- Improving face detection accuracy using deep learning models.
- Adding support for multiple cameras.
