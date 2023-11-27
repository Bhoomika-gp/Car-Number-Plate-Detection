# Car Number Plate Detection using OpenCV
## Overview
This Python project implements a real-time car number plate detection system using OpenCV. It utilizes Harcascade classifiers for detecting license plates in live video streams captured through a webcam.

## Prerequisites
Python 3.x
OpenCV (cv2)
Webcam (for live plate detection)
## Installation
1. Clone the repository:
```bash
https://github.com/Bhoomika-gp/Car-Number-Plate-Detection.git

```
2. Install the required libraries:
```bash
pip install opencv-python
```

3. Download the pre-trained Harcascade XML file (haarcascade_russian_plate_number.xml) and place it in the model directory.

## Usage
1. Run the script:
```bash
python number_plate.py
```
2. The webcam window will open, displaying the live video stream.
3. As the video runs, the system will detect license plates in the frames and draw rectangles around them. The detected plate regions will be highlighted as "Number Plate".
4. Press the 's' key to save the cropped image of the detected plate. The saved images will be stored in the plates directory.

## Project Structure
```
car-number-plate-detection/
│
├── model/
│   └── haarcascade_russian_plate_number.xml  # Pre-trained model file for plate detection
│
├── plates/
│   └── scanned_img_0.jpg  # Sample detected plate images 
│   └── scanned_img_1.jpg
│   └── ... (additional detected plate images)
│
├── LICENSE                   # File specifying the project's license (e.g., MIT License)
├── README.md                 # Project README file
├── easy_OCR.ipynb            # Jupyter Notebook for Optical Character Recognition (OCR)
├── number_plate.py           # Python script for car number plate detection
└── requirements.txt          # File listing project dependencies

```
## Additional Notes

The minimum area threshold for plate detection can be adjusted in the script (min_area variable).
Experiment with different cascade models or tuning parameters for improved plate detection accuracy.
Consider adding post-processing steps for character segmentation and optical character recognition (OCR) to extract text from detected plates.
## License
This project is licensed under the MIT License.

## Contribution
Contributions are welcome! Feel free to open issues or submit pull requests for enhancements or bug fixes.
