# Human Pose Estimation App using OpenCV
This repository contains a Streamlit application that performs human pose estimation using OpenCV. The app takes an image as input and estimates the pose of any humans in the image.

## How it works
The app uses a pre-trained deep learning model to detect key body joints in the input image. The model is based on the OpenPose architecture and is implemented using OpenCV's DNN module. It leverages the power of deep learning and computer vision to estimate human poses in images. Here's a breakdown of the process:

1. **Image Preprocessing:** The input image is resized and normalized to prepare it for the deep learning model. This ensures that the image is in the correct format and scale for the model to process.

2. **Pose Estimation Model:** The core of the app is a pre-trained OpenPose model. This model is a Convolutional Neural Network (CNN) that has been trained on a massive dataset of images with labeled human poses. It can accurately detect key body joints like wrists, elbows, knees, and ankles.

3. **Joint Detection:** The model analyzes the input image and predicts the location of various body joints. It outputs a set of confidence maps and part affinity fields (PAFs). Confidence maps indicate the probability of a joint being present at each pixel, while PAFs encode the association between body parts.

4. **Pose Construction:** The app uses a sophisticated algorithm to assemble the detected joints into a coherent human pose. This involves analyzing the confidence maps and PAFs to identify connections between joints and construct a skeletal representation of the human body.

5. **Visualization:** Finally, the app overlays the estimated pose on the original image, providing a clear visualization of the detected body joints and connections. This allows you to see how the model has interpreted the human pose in the image.

## Input image
![stand](https://github.com/user-attachments/assets/5acf80bd-717d-465f-b09e-46eb2952b54f)

## Output image
![output-image](https://github.com/user-attachments/assets/42f9637e-0754-4c1f-8a13-4bb1326c375b)

## How to use
#### 1. Clone the repository:
      git clone https://github.com/imvarun18/Human-pose-estimation.git

#### 2. Install the required packages:
      pip install -r requirements.txt

#### 3. Run the app:
      streamlit run estimation_app.py
   
#### 4. Upload an image or use the demo image.
   
#### 5. The app will display the original image and the estimated pose.

## Requirements
1. Python 3.7 or higher
2. OpenCV
3. Streamlit
4. Pillow
5. Matplotlib
6. Pandas
