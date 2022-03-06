# Social Distancing Detection

#### Technologies | Computer Vision
#### Domain | Healthcare, Public Safety

## Problem Statement:
##### Social distancing detection using deep learning to evaluate the distance between people to mitigate the impact of this coronavirus pandemic. The detection tool was developed to alert people to maintain a safe distance with each other by evaluating a video feed. The video frame from the camera was used as input, and the open-source object detection pre-trained model

## Implementation 
- YOLO  trained on COCO dataset is used to detect people from camera frame as input
- After detecting people pairwise distance is calculated between all detected people
- Based on the computed distances, we determine whether social distancing rule is being violated or not.(here distince is used in pixels, minimum = 50 )

## Installation

1. Clone the git reprository
```bash
$ git clone https://github.com/KalyaniAvhale/social-distance-detection.git
$ cd social-distance-detection
```

2. Install dependencies
```bash
$ pip install -r requirements.txt 
```

3. Run social_distance_detection.py file (input will be webcam by default to input local file use --input TestVideo.mp4)
```bash
$  python social_distance_detection.py --input TestVideo.mp4
```


