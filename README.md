# License Plate Detector
The plate_detector.cpp program is a license plate detector that utilizes the OpenCV library. It captures video from the default camera and detects license plates in real-time using a pre-trained Haar cascade classifier specifically designed for Russian license plates.

## Features
* Real-time License Plate Detection: The program continuously captures frames from the camera and detects license plates using the loaded Haar cascade classifier.
* Saving Detected Plates: When a license plate is detected, the corresponding region of interest (ROI) is cropped and saved as an individual image in the "Plates" folder within the "Resources" directory.
* Visualization: Detected license plates are highlighted with a purple rectangle on the original video feed.

## Requirements
* C++ compiler
* OpenCV library

## Usage
1. Clone the repository: git clone https://github.com/jakubpiwowarski/plate_detector_cpp.git
2. Navigate to the project directory: cd license-plate-detector
3. Compile the source code: g++ plate_detector.cpp -o plate_detector pkg-config --libs opencv``
4. Run the program: ./plate_detector

## How It Works
1. The program initializes the camera to capture video frames.
2. It loads the pre-trained Haar cascade classifier specifically designed for Russian license plate detection.
3. In an infinite loop, the program continuously captures frames from the camera.
4. The Haar cascade classifier is applied to each frame to detect license plates.
5. For each detected license plate, the corresponding region of interest (ROI) is cropped and saved as an individual image in the "Plates" folder.
6. The original video feed is displayed with purple rectangles drawn around detected license plates.


## Contributing
Contributions are welcome! If you find any issues or have ideas for improvements, please open an issue or submit a pull request.
