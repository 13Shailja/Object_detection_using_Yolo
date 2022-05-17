# Object_detection_using_Yolo
A project for the detection of objects using Yolo

![image](https://user-images.githubusercontent.com/50164374/168779064-8107e076-f42e-48e1-93bc-b9312c65cba0.png)

This repository is the subsection of the Project proposed, **Image-Adaptive YOLO for Object Detection in Adverse Weather Conditions**

The repository consists of working code for the Object Detection using YOLO.

## Technical Papers
Study Papers can be found at the below location:

1. [Yolo Paper](Study_Papers/Yolo_Paper.pdf)
2. [Image Adaptive Yolo Paper](Study_Papers/Image_Adaptive_YOLO_for_Object_Detection_in_Adverse_Weather_Conditions.pdf)

## Steps of executing the Yolo Detection program
1. Converting the darknet weights to tensorflow:
  Execute the [save_model.py](Code_for_Object_Detection/save_model.py)
  This step will save the weights on the local machine in the "checkpoints" folder
  
  
2. To execute the object detection on Image files:
  Execute the [detect.py](Code_for_Object_Detection/detect.py)
  We need to send the parameters so the python file can select the appropriate model
  Sample Execution statement: python detect.py --weights ./checkpoints/yolov4-416 --size 416 --model yolov4 --images ./data/images/catsAndDogs.jpg
  
  
3. To execute the object detection on Video files:
  Execute the [detect_video.py](Code_for_Object_Detection/detect_video.py)
  We need to send the parameters so the python file can select the appropriate model
  Sample Execution statement: python detect_video.py --weights ./checkpoints/yolov4-416 --size 416 --model yolov4 --video ./data/video/Chicago.mp4 --output ./detections/outputOfChicago_demo.mp4
  
  ## Learning Goal
  The outcome of this project, gave me following insights:
  * Successfully used "OpenCv" for the image processing
  * Understood the Bounding Boxes and ROI (Region of Interest)
  * Was able to understand the Convolutional layers
  
  ## Further work
  * Understanding the advanced Computer Vision for the Image pre-processing
  * Enhanching the characteristics of Yolo to detect objects in low-light and foggy images.
