# Car Tracking System Using Python

## Overview

This project involves implementing a car tracking system using Python, leveraging powerful libraries such as OpenCV and NumPy. The primary goal is to detect and track cars in video feeds and analyze traffic data by counting cars and calculating their average rate per minute.

## Key Features

    - Object Tracking with Kalman Filter: Utilizes a Kalman filter within a Tracker class to predict and track the movement of cars with improved accuracy.
    - Video Frame Processing: Processes video frames to enhance contour detection using techniques like Gaussian blur and morphological operations.
    - Traffic Data Analysis: Counts cars heading in specific directions and calculates traffic metrics such as the average rate of cars per minute.

## Installation

    1. Set up the environment: Ensure that you have Python and pip installed on your system.

    2. Install the necessary packages:

   pip install opencv-python numpy tabulate

Make sure the required libraries are installed, specifically opencv-python, numpy, and tabulate.

## Usage

    1. Import required packages:

   import cv2
   import numpy as np
   import tabulate

    2. Run the main code:

    Create a Tracker class instance and utilize it in a video feed to track cars.

    3. Analyze Video:

    Use the function count_cars_going_left(file: str, debug=False) to analyze video files, which will output the total number of cars and cars per minute.

## How It Works

    - Kalman Filter in Tracking: The Tracker class uses a Kalman filter to - predict car movements. It maintains a history of centroids and uses linear regression to determine the direction (left or right) of car movement.

    - Contour and Centroid Calculation: The code calculates the centroids of detected contours to establish the position of cars and updates the tracking data.

    - Traffic Analysis: The system can compute car counts and traffic flow rates by analyzing frames over time, providing insights into traffic patterns.

## Sample Results

The program includes predefined video files for testing, which are analyzed for traffic patterns with results summarized in a tabulated format.

## Conclusion

This project provides a robust foundation for developers interested in computer vision applications in traffic monitoring, facilitating the development of advanced vehicle tracking systems.

Feel free to contribute by improving the detection algorithms or extending functionality to track different vehicle types or additional features.

Thank you for using this car tracking system! If you encounter any issues or have suggestions, please open an issue on GitHub.
