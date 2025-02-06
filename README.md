# Human Pose Estimation App using OpenCV
This repository contains a Streamlit application that performs human pose estimation using OpenCV. The app takes an image as input and estimates the pose of any humans in the image.

## How it works
The app uses a pre-trained deep learning model to detect key body joints in the input image. The model is based on the OpenPose architecture and is implemented using OpenCV's DNN module.

## How to use
1. Clone the repository:
   git clone https://github.com/your-username/human-pose-estimation.git

2. Install the required packages:
   pip install -r requirements.txt
   
3. Run the app:
   streamlit run estimation_app.py

4. Upload an image or use the demo image.

5. The app will display the original image and the estimated pose.

## Requirements
Python 3.7 or higher
OpenCV
Streamlit
Pillow
Matplotlib
Pandas
