# Einstein Vision - Checkpoint 1 Submission

This repository contains the code and data for the RBE 549: Computer Vision project, Einstein Vision, completed by Irakli Grigolia and Tupak Nagle. The goal of this project is to implement various computer vision techniques to detect and analyze the environment around a moving car. 

## Networks Utilized

The project utilizes the following networks:

1. Object Detection (cars, traffic signs, traffic lights, speed limit sign): A TensorFlow-based object detection model from [xiaogangLi/tensorflow-MobilenetV1-SSD](https://github.com/xiaogangLi/tensorflow-MobilenetV1-SSD) is used to detect objects in the scene. The midpoints of the bounding boxes are used to identify the position of cars, traffic signs, and traffic lights. Instance/panoptic segmentation network is planned to be used for better depth estimation in future iterations.

2. Depth Estimation: A transformer-based midas model from [jankais3r/Video-Depthify](https://github.com/jankais3r/Video-Depthify) is used to estimate the depth of the objects in the scene. The average depth is calculated within the region defined by the bounding boxes from object detection. Instance segmentation is planned to be used for better results in future iterations.

3. Lane Detection: YOLO Pv2 from [CAIC-AD/YOLOPv2](https://github.com/CAIC-AD/YOLOPv2) is used to detect lanes in the scene.


## References

The repository also includes references to other object detection and keypoint detection models utilized during the project.

- Lane Detection: [IrohXu/lanenet-lane-detection-pytorch](https://github.com/IrohXu/lanenet-lane-detection-pytorch)
- Monocular Depth Estimation: [isl-org/MiDaS](https://github.com/isl-org/MiDaS)
- Object Detection: Cars, Trucks, Traffic Lights, Road Signs: [xiaogangLi/tensorflow-MobilenetV1-SSD](https://github.com/xiaogangLi/tensorflow-MobilenetV1-SSD)
- Object Detection: Cars, Trucks, Traffic Lights, Road Signs: [WongKinYiu/yolov7](https://github.com/WongKinYiu/yolov7)
- Object Detection: Traffic Lights: [sovit-123/TrafficLight-Detection-Using-YOLOv3](https://github.com/sovit-123/TrafficLight-Detection-Using-YOLOv3)
- Object Detection: Road Signs: [Anantmishra1729/Road-sign-detection](https://github.com/Anantmishra1729/Road-sign-detection)
- YOLO 3-D bounding boxes: [ruhyadi/YOLO3D](https://github.com/ruhyadi/YOLO3D)
- Pedestrian keypoint detection: [ZheC/Realtime MultiPerson Pose Estimation](https://github.com/ZheC/Realtime-Multi-Person-Pose-Estimation) 

