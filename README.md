# Traffic Signal Violation Detection System

A Python-based system to detect traffic signal violations using computer vision and a graphical user interface (GUI).

---

## Features

- **Vehicle Detection**: Detects and classifies vehicles using YOLOv3.
- **Violation Detection**: Identifies traffic violations when vehicles cross a user-drawn signal line during a red signal.
- **Graphical User Interface**: Easy-to-use GUI for loading videos, marking regions of interest, and displaying results.

---

## Getting Started

### Prerequisites
- Python 3.x
- Required libraries: TensorFlow, OpenCV, NumPy, Tkinter, ImageIO
- YOLOv3 weights file (`yolov3.weights`)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Traffic-Signal-Violation-Detection-System.git
   cd Traffic-Signal-Violation-Detection-System
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Download the YOLOv3 weights file (`yolov3.weights`) and place it in the project directory.

## Usage
### Running the GUI
1. Open the terminal and activate your virtual environment.
2. Navigate to the project directory.
3. Run the GUI script:
    ```bash
    python Project-GUI.py
    ```
4. Use the GUI to:
    - Open a video file.
    - Draw the traffic signal line by selecting the Region of Interest.
    - Monitor violations in the loaded video.

### Output
- Detected violations will be highlighted with bounding boxes.
- A processed video (`output.mp4`) will be saved in the `Resources/output/` folder.

## Project Overview
- **Object Detection**: Powered by YOLOv3 for accurate vehicle classification and detection.
- **Violation Rules**: A violation is detected when a vehicle crosses the signal line during a red light.
- **GUI**: Provides a seamless interface to interact with the system without editing code.