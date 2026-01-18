Vehicle Tracking and Counting Using YOLOv8 and OpenCV
1. Project Overview

This project is developed to detect, track, and count vehicles when they cross a predefined virtual line in a video.
It uses YOLOv8 for object detection and OpenCV for video processing and visualization.

The system keeps track of each vehicle and increments the count only when the vehicle crosses the line, avoiding duplicate counts.

2. Objective of the Project

To detect vehicles from video input

To track each vehicle uniquely across frames

To count vehicles accurately when they cross a specific line

To provide a simple and efficient traffic analysis solution

3. Technologies Used

Python – main programming language

YOLOv8 (Ultralytics) – for vehicle detection

OpenCV – for video processing and drawing

NumPy – for numerical operations

PyTorch – backend for YOLOv8

4. How the System Works (Step by Step)

A video or webcam feed is taken as input.

Each frame is passed to the YOLOv8 model.

YOLOv8 detects vehicles such as cars, buses, and trucks.

A tracker assigns a unique ID to each detected vehicle.

A virtual counting line is defined in the frame.

When a tracked vehicle crosses the line:

Its ID is checked

The count is increased only once per vehicle

The total vehicle count is displayed on the video output.

5. Features of the Project

Real-time vehicle detection

Unique ID-based vehicle tracking

Line crossing detection

Accurate vehicle counting

Works with recorded videos or live camera feed

Lightweight and easy to modify

6. Project Folder Structure
vehicle-tracking-counting/
│
├── models/          # YOLOv8 model files
├── videos/          # Input videos
├── outputs/         # Output videos or images
├── src/             # Source code files
│   ├── main.py
│   ├── tracker.py
│   └── counter.py
│
├── requirements.txt
├── README.md
└── .gitignore

7. Installation Steps

Clone the repository:

git clone https://github.com/yourusername/vehicle-tracking-counting.git


Move into the project directory:

cd vehicle-tracking-counting


Install required libraries:

pip install -r requirements.txt

8. How to Run the Project

Run the main Python file:

python src/main.py


If your program uses a video file:

python src/main.py --video videos/sample_video.mp4

9. Output

Bounding boxes around detected vehicles

Vehicle ID displayed on each vehicle

Counting line visible in the frame

Total vehicle count displayed on screen

(You can add screenshots or demo videos here)

10. Applications of the Project

Traffic monitoring systems

Smart city applications

Road congestion analysis

Toll booth automation

Surveillance and security systems

11. Limitations

Performance depends on video quality

Accuracy may reduce in heavy traffic or occlusion

Works best in fixed camera scenarios

12. Future Enhancements

Vehicle speed estimation

Multi-line or multi-lane counting

Vehicle classification (car, bus, truck, bike)

Web or dashboard-based visualization

Database integration for analytics

13. Conclusion

This project demonstrates how computer vision and deep learning can be used to solve real-world traffic monitoring problems.
It is scalable, customizable, and suitable for academic and real-world applications.

14. Credits

YOLOv8 by Ultralytics

OpenCV community

Python open-source ecosystem
