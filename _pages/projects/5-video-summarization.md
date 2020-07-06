---
featured: true
button: "btn btn--primary btn--x-large"
layout: splash
title: "AI Video Summarization"
permalink: /video-summarization/
description: "Summarization tool for security camera footage using neural network object detection"

header:
  overlay_color: "#000"
  overlay_filter: "0.80"
  overlay_image: /assets/media/video-summarization/banner.png

excerpt: "This python tool takes a large amount of input security camera footage and outputs a dramatically shortened version where relevant are events are overlayed simultaneously.

>Created by: Henry Luengas, Kevin Vincent, Oliver Curry, Ritwik Kesavath, and Christopher Creber"

video_row1:
  - video_path: /assets/media/video-summarization/Day_One.webm
    title: "Project Idea & Goals"
    excerpt: "This python tool was a group project for an artificial intelligence course; its inspiration came from the comercial product called [*BriefCam*](https://www.briefcam.com/). The goal of the project was to improve the experience of reviewing security camera footage. Security cameras generally either produce continuous footage, or a set of shorter clips containing significant motion, or detected objects. The system we produced can improve the review experience of either of these types of inputs. It works by taking any number of footage clips and combining them into a single clip of the same length. The following examples come from my inexpensive front door camera, representing an incresingly common use case. These three one-minute summarizations are combinations of all the one-minute clips containing motion over two daily periods and one night-time period."


video_row2:
  - video_path: /assets/media/video-summarization/Day_Two.webm
    title: "Object Detection: YOLO & OpenCV"
    excerpt: "Any detected objects that moved significantly, are all overlayed in the summary clip so that the viewer recieves a highly condensed version of all the clips. People, vehicles, and about 90 other classes of objects can be detected using the YOLO object detection network that was pre-trained on the COCO dataset. Without a GPU for image detection, the tool was only able to process footage at a *real-time* rate while processing every fifth frame of video, making it only useful to the extent that computer time is less valuable than a human's. However, when paired with a powerful GPU or other specific neural network optimized hardware, the tool would be a legitimate timesaver for reviewing critical security camera footage.
    

    We decided to use YOLOv3 because it produced very accurate results for the type of objects we cared about, namely people and vehicles, using poor quality cheap security camera footage. One unfortunate result of this is we did not recieve the valuable and difficult experience of training our own neural network. Most other groups focused on this aspect, whereas the majority of our project involved manipulating and tracking image data. This was mostly done using OpenCV, an open source computer vision and image proccessing library." 

    

video_row3:
  - video_path: /assets/media/video-summarization/Night_One.webm
    title: "Implementation Pipeline"
    excerpt: "

The proccess runs as five stage a pipeline: 
    
### Detector Stage: \n
This stage runs YOLOv3 on every 5 input frames, bounding boxes are stored for detections with confidence levels over 30%. This bounding box data is serialized into a file so that future stages can be processed without having to re-run the detector. 

### Track Stage: \n
The previous stage generates a large array that contains the detections for many frames of the input video. The track stage passes this information into an open source object tracker. This object tracker computes and interpolates *tracks*. Tracks are made up of unique objects and their respective paths through the frames in which they appear.

### Filter Motion Stage: \n
This stage filters down the tracks above to only tracks that move more than a certain threshold. This keeps static detected objects out of the final summarization.

### Frame Assign Stage: \n
The output of the previous stage is a mapping of each unique object to the frames in which it appears and its location. In order to visualize the output we need the opposite mapping. That is, given a frame number, we need the unique objects and their bounding boxes. This step computes that mapping.

### Visualize Stage: \n
The output of the previous stage is a mapping of frame number to unique, moving objects in the frame and their positions. This stage reads in the video files and draws bounding boxes onto each frame in which we have identified objects then writes them to the output video file.
"


---

<div style="text-align: justify">

{% include video_row id="video_row1" type="right" %}
{% include video_row id="video_row2" type="right" %}
{% include video_row id="video_row3" type="right" %}

</div>