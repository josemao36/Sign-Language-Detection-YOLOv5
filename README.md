# Sign-Language-Detection-YOLOv5
A real-time sign language detection model using YOLOv5 and PyTorch. Capable of recognizing the ASL alphabet from a webcam feed
Real-Time Sign Language Detection with YOLOv5
This project is a computer vision application that uses the YOLOv5 model to detect and recognize American Sign Language (ASL) gestures in real-time from a webcam feed.

<!-- You can add a GIF of your project working here later -->

Features
Real-time detection and classification of ASL alphabet signs.

Built using the powerful YOLOv5 architecture.

Trained on a custom dataset of sign language gestures.

Technologies Used
Python 3.9

PyTorch

YOLOv5 (v7.0)

OpenCV

Dataset
This model was trained on a custom dataset sourced from Roboflow. You can find the dataset here:
Sign Language ASL Roboflow Dataset

Installation & Setup
Clone the repository:

git clone https://github.com/YourUsername/Sign-Language-Detection-YOLOv5.git
cd Sign-Language-Detection-YOLOv5

Create and activate a conda environment:

conda create --name sign_language_env python=3.9 -y
conda activate sign_language_env

Install the required libraries:

pip install -r requirements.txt

How to Run
To run the real-time detection on your webcam, place the best.pt model file in the main directory and run the following command:

python detect.py --weights best.pt --source 0

Important Note
The file models/experimental.py has been modified to handle a PosixPath error that occurs when loading a model trained on a Linux-based system (like Google Colab) on a Windows machine. This change is necessary for the model to load correctly.

Acknowledgements
This project is built upon the official YOLOv5 repository by Ultralytics.
