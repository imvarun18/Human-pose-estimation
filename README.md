# Human Pose Estimation App using OpenCV
This repository contains a Streamlit application that performs human pose estimation using OpenCV. The app takes an image as input and estimates the pose of any humans in the image.

## How it works
The app uses a pre-trained deep learning model to detect key body joints in the input image. The model is based on the OpenPose architecture and is implemented using OpenCV's DNN module.

## How to use
Clone the repository:
Bash

git clone https://github.com/your-username/human-pose-estimation.git
Install the required packages:
Bash

pip install -r requirements.txt
Run the app:
Bash

streamlit run estimation_app.py
Upload an image or use the demo image.
The app will display the original image and the estimated pose.

## Requirements
Python 3.7 or higher
OpenCV
Streamlit
Pillow
Matplotlib
Pandas
